# Développement d'un évaluateur d'états mémoire pour programmes en bytecode Java Card.

## abstract
Java Card est un sous ensemble de Java adapté pour les cartes à puces.
Une carte à puce charge un fichier CAP résultant de la transformation
des applets, et exécute le bytecode Java Card du fichier à l’aide de la
Machine Virtuelle Java Card (JCVM) composée de zones mémoires où les
changements seront affectés.

Les composants de la mémoire d’une JCVM sont un tas, les registres,
des zones de méthodes et une pile (JCVM Stack) associée à chaque thread.
Une JCVM stack contient plusieurs frames où chaque frame est composée
d’une pile d’opérandes avec son registre associé (SP register), un tableau
des variables locales et le code de la méthode en cours d’exécution avec
son registre associé (PC register).

Dans le présent travail, on a développé un outil qui simule, partiellement,
le fonctionnement de la JCVM. Il s’agit d’un évaluateur d’état
mémoires qui prend en entrée un fichier CAP et fournit pour chaque instruction
interprétée, l’état mémoire correspondant.

Mot clés : Machine Virtuelle Java Card (JCVM), fichier CAP, bytecode
Java Card, état mémoire.
