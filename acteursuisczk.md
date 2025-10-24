classDiagram
    Acteur <|-- Auteur
    Acteur <|-- Lecteur
    Acteur <|-- Plateforme_archives
    Acteur : +langue, langues principales
    Acteur : +période activité [années]
    Acteur : +peut interagir sur plateforme()
    Acteur : +a accès au texte()
    class Auteur{
      +langue d'expression
      +nombre de textes publiés
      +écrit et édite le texte()
      +écrit et édite les paradonnées et tags()
    }
    class Lecteur{
      +langue des textes favorisés
      +tags et paradonnées favorisées
      +lit les textes > incidence sur score des textes()
      +favorise des textes selon les paradonnées et tags()
    }
    class Plateforme_archives{
      +ensemble des langues
      +ensemble des paradonnées et tags
      +nombre de textes hébergés
      +héberge les textes()
      +donne accès aux textes aux utilisateurs()
    }
