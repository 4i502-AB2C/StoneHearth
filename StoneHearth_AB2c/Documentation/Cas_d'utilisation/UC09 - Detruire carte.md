# UC22 - Détruire une carte
9/10/2017

## Description:
Le joueur détruit une carte pour avoir des joyaux

## Acteurs:
Joueur

## Pre-conditions
(Aucune)

## Sequencement nominal
1. Le joueur décide de détruire une carte
2. Le système affiche les cartes que le joueur a en double
3. Le joueur choisit une carte
4. Le système vérifie le prix à partir de la rareté de la carte
5. Le système affiche le prix de la carte et demande une confirmation de destruction
6. Le joueur confirme détruire la carte
7. Le système retire le doublon de la collection du joueur et ajoute les joyaux au porte-monnaie du joueur
8. Le système demande à l'utilisateur s'il veut acheter d'autres cartes
9. Le joueur décline

## Post-conditions
La carte n'est plus dans la collection du joueur
Le joueur a un porte-monnaie augmenté du prix de destruction de la carte

## Alternatives
A1 - Le joueur veut détruire d'autres cartes
L'alternative démarre après SN.8
    9. Le joueur accepte
    10. Retour à SN.2

## Exceptions
E1 - Annulation
L'exception démarre après SN.2 ou SN.6
    1. Le joueur décide d'annuler la destruction
