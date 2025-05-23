# Blockchain


Objectifs pédagogiques
- Rendre une donnée infalsifiable et sécurisée
- Implémenter une blockchain simplifiée en Python
- Comprendre le fonctionnement de la preuve de travail (Proof of Work)
- Découvrir l'utilité des arbres de Merkle pour l'intégrité des données
- Simuler la décentralisation avec plusieurs nœuds sur une même machine
- Tester la résilience face à une attaque des 51 %
- Détecter les corruptions de chaînes distribuées  

  
Étape 1 : Création d’un bloc et de la chaîne
Classe Block
Classe Blockchain
(Programmation orientée objet facultative mais recommandée)  

Travail demandé :
Écrire le code de base pour créer une blockchain avec blocs chaînés par hash.  


Étape 2 : Ajout de la preuve de travail (PoW)
Implémenter le mécanisme de minage via PoW
Travail demandé :
Rendre le minage de blocs coûteux, observer l’impact sur le temps de calcul.


Étape 3 : Arbre de Merkle
Implémenter une méthode compute_merkle_root
Créer un arbre binaire à partir des hash des blocs  

Travail demandé :
Afficher & comparer visuellement l’arbre ou sa racine.  


Étape 4 : Simulation de décentralisation
Créer x instances de la même chaine avec x%2==1  

Travail demandé :
Simuler 5 instances pour l'instant identiques  


Étape 5 : Simulation d'une attaque à 51 %
Corrompre un noeud, puis x/2 + 1

Travail demandé :
Observer le résultat : la majorité écrase-t-elle la minorité ? Une chaîne corrompue peut-elle
prendre le dessus ?  


Étape 6 : Détection de corruption (intégrité distribuée)
Chaque instance doit pouvoir être validée individuellement et par rapport à l'intégralité de la
chaine
Vérification des hash
Vérification de la racine Merkle  

Travail demandé :
Ajouter un mécanisme de rejet automatique d'une chaîne corrompue. Observer ce qu’il se passe
si un seul instance triche.  


Contraintes supplémentaires
Pas d’écriture dans des fichiers : tout reste en mémoire
Pas de bibliothèque externe sauf hashlib & time
Faire le plus de cas de tests possibles : corruption de data seule, de bloc, de chaine, de chaines,
etc.
