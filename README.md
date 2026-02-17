# PhonePro - Annuaire Téléphonique

Une application Java simple et efficace pour gérer vos contacts téléphoniques via une interface console.

##  Fonctionnalités

-  **Lister les contacts** - Afficher tous les contacts enregistrés
-  **Ajouter un contact** - Créer un nouveau contact avec nom, prénom et numéro
-  **Supprimer un contact** - Supprimer un contact par son numéro de téléphone
-  **Persistance des données** - Sauvegarde automatique dans un fichier texte

##  Technologies

- **Java 14+**
- **Maven** pour la gestion des dépendances
- **Architecture en couches** (Model-Repository-Service-UI)

##  Prérequis

- Java JDK 14 ou supérieur
- Maven 3.6+

##  Installation et Exécution

1. **Cloner le projet**
```bash
git clone https://github.com/kvill01/annuaire-java-console.git
cd annuaire-java-console
```

2. **Compiler le projet**
```bash
mvn compile
```

3. **Exécuter l'application**
```bash
mvn exec:java -Dexec.mainClass="bf.annuaire.Main"
```

Ou alternativement :
```bash
java -cp target/classes bf.annuaire.Main
```

##  Utilisation

Au lancement, un menu interactif s'affiche :

```
==== ANNUAIRE TELEPHONIQUE ====
1. Lister les contacts
2. Ajouter un contact
3. Supprimer un contact
4. Quitter
Votre choix :
```

### Ajouter un contact
- Sélectionnez l'option 2
- Saisissez le nom, prénom et numéro de téléphone
- Le contact est automatiquement sauvegardé

### Supprimer un contact
- Sélectionnez l'option 3
- Entrez le numéro de téléphone du contact à supprimer

##  Structure du Projet

```
src/main/java/bf/annuaire/
├── Main.java                    # Point d'entrée de l'application
├── model/
│   └── Contact.java            # Modèle de données Contact
├── repository/
│   └── ContactRepository.java  # Gestion de la persistance
├── service/
│   └── ContactManager.java     # Logique métier
└── ui/
    └── ConsoleUI.java          # Interface utilisateur console
```

##  Stockage des Données

Les contacts sont sauvegardés dans le fichier `contacts.txt` à la racine du projet. Ce fichier est créé automatiquement lors du premier ajout de contact.

##  Tests

Pour exécuter les tests :
```bash
mvn test
```

##  Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
- Signaler des bugs
- Proposer de nouvelles fonctionnalités
- Améliorer la documentation

##  Licence

Ce projet est sous licence libre. Vous pouvez l'utiliser, le modifier et le distribuer librement.

---
**Sawadogo Abdel Kaled** - [GitHub](https://github.com/kvill0780)

---

⭐ N'hésitez pas à donner une étoile si ce projet vous a été utile !
# annuaire-java-console
