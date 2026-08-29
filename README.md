# Implémentation de l'algorithme de signature DSA (FIPS 186-3)

## Contexte et objectifs du projet
Ce projet de Master 2 consiste à implémenter l'algorithme de signature numérique **DSA (Digital Signature Algorithm)** en se basant sur le standard **FIPS 186-3 (Section 4)**. 

## Paramètres publics imposés
- $q = 2^{160} + 7$
- $p = 1 + (2^{160} + 7)(2^{864} + 218)$
- $g = 2^{(p-1)/l} \pmod p$

## Outils et technologies
- **Langage** : Java natif (JDK)
- **Environnement** : VS Code
- **Bibliothèques** : Classe `java.math.BigInteger` obligatoire, car les types primitifs (`long`, `double`) sont insuffisants pour des clés de cette taille (1024 bits et 160 bits).
- **Hachage** : SHA-3 recommandé ou hachage factice pour les tests.

## Les rendus
1. Code source Java complet et documenté.
2. Rapport d'implémentation (choix techniques).
3. Programme de Benchmark (10 000 itérations).
4. Résultats du Benchmark et spécifications de la machine.

## Utilisation
(Les commandes de compilation et d'exécution `javac` et `java` seront ajoutées ici ultérieurement).