# Gestion-bibliotheque
Ce projet est une API REST construite avec **Spring Boot** permettant de gérer les **auteurs** et leurs **livres**, en utilisant les entités JPA et les relations `@OneToMany` / `@ManyToOne`.
🛠 Technologies utilisées
Java 17
Spring Boot
Spring Data JPA
Hibernate
H2 Database
Maven
## 🚀 Lancer le projet
 ✅ Prérequis

- Java 17+
- Maven 3+
- Un IDE (IntelliJ, Eclipse, VSCode...)
- Postman (ou curl) pour tester l’API
- ▶️ **Étapes d’exécution**
- 1. Cloner ou extraire le projet :
   ```bash
   git clone https://github.com/famaniang02/Gestion-bibliotheque.git
   cd projet-bibliotheque
  **Lancer le projet**
   mvn spring-boot:run
   Par défaut, la base de données H2 est utilisée en mémoire. Vous pouvez accéder à sa console via http://localhost:8080/h2-console
   **EXEMPLE D'APPEL D'API**
   1/Creer un auteur
   POST /auteurs
   Content-Type: application/json

   {
  "nom": "Victor Hugo"
   }
   2/Ajouter un livre pour un auteur
   
   methode:POST /auteurs/1/livres
   Content-Type: application/json

    {
  "titre": "Les Misérables"
    }
   3/Lister tous les livres
   GET /livres
   exemple sur postman
   methode Get; lien:http://localhost:8080/livres
   4/Afficher les livres d'un auteur donne
   GET /auteurs/1/livres
     Exemple sur postman
   ## methode:GET lien :http://localhost:8080/livres/auteur/1
    lister tous les livres de l'auteur de l'ID 1
   5/Supprimer un livre
   ## DELETE /livres/1

   **Liste des fonctionnalites implementees**
   
   ✅ Créer, lire, mettre à jour, supprimer des auteurs

   ✅ Créer, lire, mettre à jour, supprimer des livres

   ✅ Associer un livre à un auteur

   ✅ Récupérer les livres d’un auteur donné

   ✅ Gestion des erreurs simples (ressources non trouvées)




   
   
