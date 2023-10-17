# Exercice 02 : Eleves
## durée : 45'
## Objectifs visés :
- Implémentation d’une classe simple
- Création et utilisation d‘objets stockés dans un tableau
## PARTIE 1 : Créer votre classe qui modélisera un élève
Dans ce projet vous allez créer une classe Java qui représentera **un élève**.

Dans ce projet créez une classe modélisant un `Eleve`. Un `Eleve` aura comme attributs un nom et un prénom et seulement des getters. Basez-vous sur le diagramme de classe pour les informations manquantes.

```mermaid
---
title: Diagramme de classe : Eleve
---
classDiagram

class Eleve {
    -String prenom
    -String nom
    Eleve(String prenom, String nom)
    +getNom() String
    +getPrenom() String
}
```
Au dessus du `main()`, créez une constante `NBRE_MAX_ELEVES` de valeur `20`. Celle-ci représente la taille maximale d'une classe d'élèves.

Dans votre `main()`, déclarez une variable `eleves` permettant de contenir `NBRE_MAX_ELEVES` objets de type `Eleve`. Créez ensuite cette structure de données.

Créez ensuite 5 objets différents de type `Eleve`. Placez ces élèves dans les 4 premières cases de votre tableau, laissez les deux emplacements suivants vides et placez ensuite le dernier élève.

Dans une boucle, parcourez l'ensemble de votre tableau à la recherche d'élèves et , lorsque vous en trouvez un, affichez-le sur la console de la manière suivante :
```
L'élève N°0 s'apelle => James Cameron
L'élève N°1 s'appelle => Mac Haroni
L'élève N°2 s'appelle => John D'Oeuf
L'élève N°3 s'appelle => Alex Terrieur
L'élève N°6 s'appelle => Alain Terrieur
```
## Partie 2 : Affichage de la classe par elle même
Rendez plus intelligente votre classe `Eleve` en apprenant à ses objets à s’afficher eux-mêmes de manière lisible et compréhensible.

On va faire en sorte qu’un `sout( unEleve );` affiche automatiquement son prénom et son nom séparé par un espace.

Surchargez la méthode `toString()` de votre classe Eleve pour faire ceci. Adaptez votre programme principal dans le main() pour en tirer profit.
```mermaid
---
title: Diagramme de classe : Eleve avec toString()
---
classDiagram

class Eleve {
    -String prenom
    -String nom
    Eleve(String prenom, String nom)
    +toString() String
    +getNom() String
    +getPrenom() String
}
```