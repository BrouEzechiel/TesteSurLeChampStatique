# Compteur d'instances en Java

Ce projet démontre la différence entre les variables statiques et d'instance en Java à travers une classe `Personne` qui compte le nombre total d'instances créées.

## Fichiers

- `Personne.java` - Contient la classe Personne avec un compteur statique et un compteur d'instance
- `Main.java` - Programme principal qui crée plusieurs instances de Personne et affiche les compteurs

## Fonctionnement

La classe `Personne` contient :
- `nbInstances` : variable statique qui compte le nombre total d'instances créées (partagée entre toutes les instances)
- `nbLocal` : variable d'instance qui compte le nombre de fois que l'instance a été initialisée

À chaque création d'une nouvelle Personne (dans le constructeur) :
1. `nbInstances` est incrémenté (commun à toutes les instances)
2. `nbLocal` est incrémenté (spécifique à chaque instance)
