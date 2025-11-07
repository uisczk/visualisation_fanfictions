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
    Agent : +langue:str
    Agent : +accedeFanfictions()
    Agent : +existe()
    class ProducteursMediatique{
        +createurs:str
        +diffuseurs:str
        +auctorialite
        +determinentCanon()
        +ontDroitsAuteur()
        +peuventPoursuivreAO3()
    }    
    class ProductionMediatique{
        +objetMediatiqueSource:str
        +personnages:str
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
        +genre:str
        +age:int
        +race:str
        +orientationSexuelle:str
        +region:str
        +membreFandom:str
        +accedeInterface()
        +estHumain()
        +estFan
        +contestePolicyOTW()
    }
    class AcafanChercheur{
        +affilitationAcademique:str
        +produitRecherche()
    }
    class Lecteur{
        +fanfictionsBookmarked:int
        +periodeActivite:date
        +commenteFanfictions()
        +bookmarkeFanfictions()
        +selectionneFanfictions()
        +filtreFanfictions()
        +filtreTags()
    }
    class Auteur{
        +pseudonyme:str
        +periodeActivite:date
        +aCommeFanfictions:int
        +ecritFanfictions()
        +publieFanfictions()
        +editeFanfictions()
        +editeTags()
    }
    class Benevole {
        +pseudonyme:str
        +fonction:str
        +statut:str
        +periodeActivite:date
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
        +nombreFanfictions:int
        +hebergeFanfictions()
        +proposeTags()
    }
    class Comite{
        +membres:int
        +policy:str
        +decideProjets()
        +determinePolicy()
        +assureContinuite()
    }
    class Fanfictions{
        +mots:int
        +hits:int
        +kudos:int
        +bookmarks:int
        +auteur:str
        +commentaires:int
        +tags:str
        +avertissements:str
        +categories:str
        +classification:str
        +chapitres:int
        +estEcrite()
        +estPubliee()
        +estAccessible()
        +estLue()
        +estCommentee()
        +estBookmarked()
    }
    class CorpusEtendu{
        +moyenneMots:int
        +moyenneKudos:int
        +moyenneHits:int
        +partClassifications[5]:int
        +partCategories[6]:int
    }
    class CorpusRestreint{
        +nombreFanfictions:int
        +moyenneMots:int
        +moyenneKudos:int
        +moyenneHits:int
        +partClassifications[5]:int
        +partCategories[6]:int
    }
