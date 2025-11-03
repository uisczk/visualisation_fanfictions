```mermaid
  classDiagram
    Agent <|-- ProducteursMediatique
    Agent <|-- Grassroots
    ProducteursMediatique <|-- ProductionMediatique
    Grassroots <|-- Utilisateur
    Grassroots <|-- OrganizationForTransformativeWorks_OTW
    Utilisateur <|-- AcafanChercheur
    Utilisateur <|-- Lecteur
    Utilisateur <|-- Auteur
    Utilisateur <|-- Benevole
    OrganizationForTransformativeWorks_OTW <|-- ArchiveOfOurOwn_AO3
    OrganizationForTransformativeWorks_OTW <|-- Comite
    ArchiveOfOurOwn_AO3 <|-- Fanfictions
    Fanfictions <|-- CorpusEtendu
    Fanfictions <|-- CorpusRestreint
    Fanfictions o-- Lecteur
    Fanfictions --o Auteur
    ArchiveOfOurOwn_AO3 o--o Benevole
    ArchiveOfOurOwn_AO3 o--o Auteur
    Agent : +langue
    Agent : +periodeActivite
    Agent : +accedeFanfictions()
    Agent : +existe()
    class ProducteursMediatique{
        +createurs
        +diffuseurs
        +auctorialite
        +determinentCanon()
        +ontDroitsAuteur()
        +peuventPoursuivreAO3()
    }    
    class ProductionMediatique{
        +objetMediatiqueSource
        +personnages
        +canon
        +estProduite()
        +estDiffusee()
        +estTransformableDerivable()
    }
    class Grassroots{
        +contribueFandoms()
        +estIndependant()
        +produit()
    }
    class Utilisateur{
        +genre
        +age
        +race
        +orientationSexuelle
        +region
        +membreFandom
        +accedeInterface()
        +estHumain()
        +estFan
        +contestePolicyOTW()
    }
    class AcafanChercheur{
        +affilitationAcademique
        +produitRecherche()
    }
    class Lecteur{
        +fanfictionsBookmarked
        +commenteFanfictions()
        +selectionneFanfictions()
        +filtreFanfictions()
        +filtreTags()
    }
    class Auteur{
        +pseudonyme
        +fanfictionsPubliees
        +ecritFanfictions()
        +publieFanfictions()
        +editeFanfictions()
        +editeTags()
    }
    class Benevole {
        +pseudonyme
        +fonction
        +statut
        +accedeCodeSource()
        +editeTags()
        +trieTags()
        +entretientAO3()
    }
    class OrganizationForTransformativeWorks_OTW{
        +projets[5]
        +protectionJuridique
        +fondeProjets[5]()
    }
    class ArchiveOfOurOwn_AO3{
        +nombreFanfictions
        +hebergeFanfictions()
        +proposeTags()
    }
    class Comite{
        +membres
        +policy
        +decideProjets()
        +assureContinuite()
    }
    class Fanfictions{
        +mots
        +hits
        +kudos
        +bookmarks
        +auteur
        +commentaires
        +tags
        +avertissements
        +categories
        +classification
        +chapitres
        +estEcrite()
        +estPubliee()
        +estAccessible()
        +estLue()
        +estCommentee()
        +estBookmarked()
    }
    class CorpusEtendu{
        +moyenneMots
        +moyenneKudos
        +moyenneHits
        +partClassifications[5]
        +partCategories
    }
    class CorpusRestreint{
        +nombreFanfictions
        +moyenneMots
        +moyenneKudos
        +moyenneHits
        +partClassifications[5]
        +partCategories
    }
