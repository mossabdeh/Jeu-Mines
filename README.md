**Nom :Laggoune**

**Prénom :Abd el ouadoud**

**Nom :Dehane**

**Prénom :Mosaab seif el islem**

**Fiche de gestion de la maintenance du Projet Jeu de Mines.**

**Requête :** Demande d’analyse dans le cadre d’une maintenance préventive

**Prérequis :**

**Profil du mainteneur :**

-   Compétent dans le développement d'applications Java, y compris les applications Web et de bureau, en utilisant divers frameworks et outils.
-   Quelques expériences dans le développement d'applications en utilisant C\# et .NET avec une compréhension de base de leur syntaxe et de leurs frameworks
-   Compétent dans le développement web full-stack avec une expertise en construction de bases de données
-   Une certaine exposition aux principes et méthodologies de conception UX avec une compréhension de base de la conception centrée sur l'utilisateur
-   une solide expérience en matière de tests unitaires et que vous êtes compétent(e) dans la mise en place de tests automatisés pour garantir la qualité et la stabilité du code

**Pré-analyse :**

1.  **Compréhension et familiarisation avec le projet:**
-   Objectif : Effacer un champ de mines sans faire exploser aucune mine.
-   Cliquer sur un carré avec le bouton gauche de la souris le découvre, révélant soit un nombre, soit une mine
-   Les carrés qui ne contiennent pas de mines ont un chiffre qui vous indique combien de mines se trouvent dans les carrés adjacents.
-   Cliquez avec le bouton droit de la souris sur un carré pour le marquer comme étant une mine
-   Effacez tous les carrés qui ne contiennent pas de mine pour gagner
-   Cliquez sur un carré qui contient une mine pour perdre

**Résultats Analyse structurelle :**

| **Critère de mesure** | **Embold** | **Deepsource** | **Moyenne** |
|-----------------------|------------|----------------|-------------|
| **Coverage**          | **100**    | **100**        | **100**     |
| **Total LOC**         | **367**    | **303**        | **335**     |
| **problèmes**         | **56**     | **24**         | **40**      |
| **Anti-patterns**     | **0**      | **3**          | **1.5**     |
| **Vulnérabilité**     | **1**      | **0**          | **0.5**     |

**Embold :**

**![Embold1](https://user-images.githubusercontent.com/79877072/235301837-2f3fb40b-96db-4135-9a48-d157a7875637.PNG)
**

**Deepsource :**

**![JeuMines DeepSource](https://user-images.githubusercontent.com/79877072/235301855-5c5df608-f158-41f7-a700-f9f2ed2826d1.PNG)
**

**Synthèse Analyse Structurelle :**

nous avons trouvé un total de 367 lignes de code (LOC). Cependant, nous avons également identifié 40 problèmes de code dans la base de code, qui peuvent avoir un impact négatif sur la qualité, la maintenabilité et la sécurité du logiciel.

Sur les 40 problèmes, 5 d'entre eux sont des problèmes à haut risque, ce qui signifie qu'ils peuvent causer des problèmes graves, tels que la perte de données ou des violations de sécurité. De plus, nous avons détecté 3 anti-patterns, qui sont des pratiques de programmation courantes considérées comme de mauvaises pratiques, et qui peuvent entraîner des problèmes de maintenance, de performance ou de qualité du code.

En outre, nous avons découvert 1 vulnérabilité dans la base de code, ce qui signifie que le logiciel est exposé à des menaces potentielles de sécurité, et que les attaquants peuvent exploiter cette vulnérabilité pour accéder sans autorisation, modifier ou voler des données ou effectuer d'autres activités malveillantes.

Sur la base de ces résultats, nous recommandons que l'équipe de développement aborde ces problèmes et vulnérabilités afin d'améliorer la qualité, la fiabilité et la sécurité du logiciel.

**Résultats Inspection Manuelle :**

| **Ressources évaluées**          | **Avis**                                                                                                                                                                                                                                                                               |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Code source**                  | Il y a une certaine duplication de code dans la méthode newGame(), et Il n'y a pas de gestion des erreurs dans ce code,                                                                                                                                                                |
| **Documentation**                | Il y a 2 classes non documentées, 5 méthodes non documentées et un constructeur non documenté.                                                                                                                                                                                         |
| **Structure du** **projet**      | Le projet a une structure très simple, composée uniquement de deux classes, l'une pour la fonction principale et l'autre pour la logique du jeu. Bien que cela rende le projet facile à comprendre et à maintenir, cela peut être limitant pour le développement ou l'extension future |
| **L'absence de tests unitaires** | Les tests unitaires sont indisponibles dans le projet, ce qui rend la vérification du respect des spécifications difficile.                                                                                                                                                            |

**Synthèse de l’analyse personnelle :**

Après l'inspection du code source de ce projet, nous constatons que le code présente plusieurs problèmes et vulnérabilités. Plusieurs parties du code sont mal structurées, mal documentées et difficiles à comprendre. Nous avons également identifié des vulnérabilités de sécurité qui pourraient mettre en danger les données sensibles de l'application. En conséquence, nous recommandons fortement une maintenance préventive pour améliorer la qualité, la fiabilité et la sécurité de ce projet.

**Post-Analyse :**

**Interprétation des Résultats (des deux analyses) et synthèse :**

Suite à l'analyse automatisée et manuelle du projet, nous avons pu constater plusieurs points importants. Tout d'abord, la qualité globale du code laisse à désirer, avec des problèmes de fiabilité, de complexité et de maintenabilité. En outre, le code ne suit pas les bonnes pratiques de programmation orientée objet, ce qui peut rendre la compréhension et la maintenance du code plus difficiles.

De plus, l'absence de documentation ou de tests unitaires rend la vérification et la compréhension du code plus difficile, ce qui peut affecter négativement sa qualité et sa fiabilité. Enfin, le code contient de nombreux éléments complexes, tels que des boucles imbriquées et des conditions complexes, ce qui le rend difficile à suivre et à comprendre.

En résumé, l'analyse du projet a révélé des problèmes importants de qualité, de complexité et de maintenabilité du code, ainsi que l'absence de bonnes pratiques de programmation orientée objet et de tests unitaires. Ces résultats soulignent la nécessité d'une refonte du code et d'une amélioration de la qualité globale du projet pour garantir sa fiabilité et sa pérennité à long terme.


![Embold2](https://user-images.githubusercontent.com/79877072/235301873-66f60626-2cd2-4438-8670-06c9045c66fd.PNG)

**Décision**

En conclusion, le projet "Jeu de Mines" nécessite une maintenance préventive pour améliorer sa qualité, sa fiabilité et sa sécurité, car il présente plusieurs problèmes de code et des vulnérabilités qui peuvent affecter négativement les performances et la sécurité du logiciel.
