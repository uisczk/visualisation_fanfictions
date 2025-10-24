```mermaid
classDiagram
    Acteur <|-- Auteur
    Acteur <|-- Lecteur
    Acteur <|-- Plateforme_archives_corpusEtendu
    Acteur : +langue, langues principales : expression ou favorisée
    Acteur : +période activité [années]
    Acteur : +peut interagir sur plateforme()
    Acteur : +a accès au texte()
    class Auteur{
      +nombre de textes publiés
      +écrit et édite le texte()
      +écrit et édite les paradonnées et tags()
    }
    class Lecteur{
      +tags et paradonnées favorisées
      +lit les textes > incidence sur score des textes : hits, kudos()
      +favorise des textes selon les paradonnées et tags()
    }
    class Plateforme_archives_corpusEtendu{
      +ensemble des langues
      +ensemble des paradonnées et tags
      +nombre de textes hébergés
      +héberge les textes()
      +donne accès aux textes aux utilisateurs()
      +discrimine par mots-clefs et catégories : fandoms, avertissements, etc()
    }

