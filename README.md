# Arbre Généalogique, Application Java Swing

Une application de bureau développée en Java permettant de créer, gérer et visualiser de manière interactive un arbre généalogique. Ce projet intègre une interface graphique fluide conçue avec la bibliothèque Swing.

## Fonctionnalités

* Gestion des Membres : Création de profils détaillés avec nom, prénom, sexe, date de naissance et de décès.
* Relations Familiales : Ajout dynamique de parents (père, mère), de conjoints (mari) et d'enfants (fils, fille).
* Algorithmes de Parenté : Recherche et affichage automatique des frères, sœurs, ancêtres et cousins d'un membre sélectionné.
* Calcul des Liens de Parenté : Détermination automatique et textuelle du lien exact de parenté reliant deux personnes de l'arbre.
* Interface Graphique Interactive : Visualisation dynamique de la structure familiale à l'aide d'un composant de type arbre (`JTree`) et d'un panneau de contrôle pour interagir en temps réel.

## Modèle POO

Le projet respecte les principes de la programmation orientée objet (POO) avec l'organisation suivante :
* `Arbre.java` : Classe pivot qui stocke la collection des membres et embarque la logique métier de recherche et de liaison généalogique.
* `Personne.java` : Classe mère abstraite contenant les attributs partagés (nom, prénom, etc.).
* `Homme.java` & `Femme.java` : Sous-classes spécialisées héritant de la classe `Personne`.
* `Date.java` : Classe utilitaire pour une gestion simplifiée du calendrier.
* `ArbreGenealogique.java` : Composant d'interface utilisateur graphique (`JFrame`, `JTree`, boutons d'action).
* `Main.java` : Point d'entrée de l'application qui instancie et lance l'interface.

## Structure du Dépôt

```text
Genealogy-Tree-Java/
├── src/
│   ├── Main.java
│   ├── Arbre.java
│   ├── ArbreGenealogique.java
│   ├── Personne.java
│   ├── Homme.java
│   ├── Femme.java
│   └── Date.java
├── compterendu.docx     # Rapport et documentation du projet
└── README.md            # Présentation de l'application
