# UC10 - Acheter une carte
9/10/2017

## Description:
Le joueur achète une carte avec des joyaux

## Acteurs:
Joueur

## Pre-conditions
Le joueur possède toutes les cartes basiques

## Sequencement nominal
1. Le joueur décide d'acheter une carte
2. Le système vérifie que le joueur a des coordonnées bancaires
3. Le système affiche les cartes que le joueur ne possède pas
4. Le joueur choisit une carte
5. Le système vérifie le prix à partir de la rareté de la carte
6. Le système vérifie que le joueur a suffisamment de joyaux
7. Le système affiche le prix de la carte et demande une confirmation d'achat
8. Le joueur confirme acheter la carte
9. Le système ajoute la carte à la collection du joueur et retire les joyaux du porte-monnaie du joueur
10. Le système demande à l'utilisateur s'il veut acheter d'autres cartes
11. Le joueur décline

## Post-conditions
La carte est dans la collection du joueur
Le joueur a un porte-monnaie réduit du prix de la carte

## Alternatives
A1 - La carte choisie est trop chère
L'alternative démarre après SN.6
    7. Le système affiche le prix de la carte et préviens que le joueur n'a pas assez
    8. Retour à SN.3
A2 - Le joueur veut acheter d'autres cartes
L'alternative démarre après SN.10
    11. Le joueur accepte
    12. Retour à SN.3

## Exceptions
E1 - Annulation
L'exception démarre après SN.3 ou SN.7
    1. Le joueur décide d'annuler l'achat
