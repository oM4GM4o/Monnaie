# Monnaie

## Expression de besoin:

Lorsque je rend la monnaie, j'aimerais ne pas avoir à réfléchir à calculer combien de billets ou de pièces je dois donner.
J'aimerais un truc pour lequel je donne le montant à payer, la somme que m'a donné mon client et qu'il m'affiche combien de billets et de pièces je dois rendre, en rendant le moins de petites pièces possibles.

Je pense à d'autres choses qu'on pourra mettre en place ensuite mais on va déjà faire cette étape, elle me simplifiera la vie.

## Specifications fonctionnelles V.3

- L'application doit prendre deux entrées en compte: le montant à payer et la somme que le client a donné
- L'application doit calculer le nombre minimal de pièces et de billets que l'on doit rendre
- L'application doit envoyer en sortie une quantité de monnaie à rendre
- La monnaie est le dollar canadien pour cette version
- L'application n'acceptera pas les billets de 100 dollar et plus

## Specifications fonctionnelles V.2

## Specifications téchniques

- Les valeurs entrées peuvent comporter uniquement des chiffres, des points et des virgules
- Les valeurs entrées peuvent avoir 2 décimales maximum
- Les valeurs entrées doivent être sous la forme suivante: xxx.xx ou xxx,xx ou xxx

## Choix des techno

J'ai décidé de choisir le langage Python pour l'application car il permet une utilisation simple peu importe le système d'exploitation (Linux, Windows, MacOS...). La sortie et l'entrée utilisateur se feront en console.

## Décisions techniques

Les valeurs et noms des piêces et des billets sont stockés dans un dictionnaire pour les rendre modifiable facilement (en cas de changement de monnaie). Cela permet aussi de creer un dictionnaire par monnaie différente (on pourrais en faire un pour le dollar américain, le dollar canadien...)

## Tests

Pour chaque champ:
- Entrer un nombre négatif
- Entrer un nombre positif
- Entrer un nombre décimal avec une virgule
- Entrer un nombre décimal avec un point
- Entrer des caractères
- Entrer un très grand nombre
- Entrer 0
- Ne rien entrer

Tester le fonctionnement:
- Entrer une somme payée plus petite que la somme à payer
- Entrer une somme payée égale à la somme à payer
- Entrer une somme payée plus grande que la somme à payer
