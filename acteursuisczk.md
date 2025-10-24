```mermaid
classDiagram
    Acteur <|-- Auteur
    Acteur <|-- Lecteur
    Acteur <|-- Plateforme_archives_corpusEtendu
    Acteur : +String langue, langues principales, langue expression
    Acteur : +int période activité [années]
    Acteur : +peut interagir sur plateforme()
    Acteur : +a accès au texte()
    class Auteur{
      +int de textes publiés
      +écrit et édite le texte()
      +écrit et édite les paradonnées et tags()
    }
    class Lecteur{
      +String tags et paradonnées favorisées
      +lit les textes > incidence sur score des textes()
      +favorise des textes selon les paradonnées et tags()
    }
    class Plateforme_archives_corpusEtendu{
      +String ensemble des langues
      +String ensemble des paradonnées et tags
      +int de textes hébergés
      +héberge les textes()
      +donne accès aux textes aux utilisateurs()
      +discrimine textes selon catégories, avertissements, etc()
    }

    
