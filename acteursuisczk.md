```mermaid
  classDiagram
    ProducteursMediatique <|-- ProductionMediatique
    ProducteursMediatique <|-- MembresProduction
    Utilisateur_AO3 <|-- AcafanChercheur
    Utilisateur_AO3 <|-- Lecteur
    Utilisateur_AO3 <|-- Auteur
    Utilisateur_AO3 <|-- Benevole
    OrganizationForTransformativeWorks_OTW <|-- ArchiveOfOurOwn_AO3
    OrganizationForTransformativeWorks_OTW <|-- Comite
    ArchiveOfOurOwn_AO3 <|-- Fanfictions
    Fanfictions <|-- CorpusEtendu
    Fanfictions <|-- CorpusRestreint
    ProductionMediatique o--o Utilisateur_AO3    
    ProductionMediatique o--o Fanfictions
    ProductionMediatique o-- Auteur
    ArchiveOfOurOwn_AO3 o-- Auteur
    ArchiveOfOurOwn_AO3 o-- Benevole
    Auteur o-- Fanfictions
    MembresProduction o-- Fanfictions

    class ProducteursMediatique{
        +createurs:str
        +diffuseurs:str
        +determinentCanon()
        +ontDroitsAuteur()
        +peuventPoursuivreAO3()
    }    
    class ProductionMediatique{
        +langue:str
        +objetMediatiqueSource:str
        +personnages:str
        +estCanon()
        +estProduite()
        +estDiffusee()
        +estTransformableDerivable()
    }
class MembresProduction{
	      +region:str
	      +membreFandom:str
        +estHumain()
        +travaille()
      	+peutProduireFanfictions()
    }    
    class Utilisateur_AO3{
        +genre:str
        +race:str
        +orientationSexuelle:str
        +region:str
        +membreFandom:str
        +accedeInterfaceAO3()
        +estHumain()
        +estFan
        +contestePolicyOTW()
    }
    class AcafanChercheur{
        +affilitationAcademique:str
	      +langue:str
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
      	+langue:str
      	+transformeCanon()
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
        +langue:str
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
        +chapitres:int-
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
