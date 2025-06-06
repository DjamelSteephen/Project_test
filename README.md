[architecture.txt](https://github.com/user-attachments/files/20626841/architecture.txt)
# Gestion de stock et de vente


🇧🇫 ECOLE POLYTECHNIQUE DE OUAGADOUGOU


🧾 Informations générales
Nom du projet : Système de gestion des stocks et des ventes
Technologies utilisées : Java, JDBC, PostgreSQL, JUnit 5
Architecture : MVC (Model ↔ DAO ↔ Service ↔ UI)
Type de livrable : Application console + génération de rapports + tests unitaires


🧠 Objectifs pédagogiques
Ce projet vise à :
Concevoir un schéma de base de données relationnelle (PostgreSQL)
Implémenter une application Java modulaire avec accès JDBC
Appliquer les principes de la POO et l’architecture en couches
Gérer les transactions de manière sûre
Écrire des tests unitaires robustes avec JUnit 5
Générer des rapports exploitables en texte ou CSV

Diagrammes de classe(Base de donnees)

![Diagramme de classe projet1](https://github.com/user-attachments/assets/c56a6e75-fd5d-452b-930e-b81498ca4eb5)

Architecture utilisée

[Uploading architecture.txprojet-stock-vente/
│
├── src/
│   ├── model/                 ← Modèles Java liés aux tables (POJOs)
│   │   ├── Produit.java
│   │   ├── Stock.java
│   │   ├── Commande.java
│   │   ├── ContientCommandeProduit.java
│   │   └── Facture.java
│   │
│   ├── dao/                   ← Accès à la base de données (JDBC)
│   │   ├── ProduitDAO.java
│   │   ├── StockDAO.java
│   │   ├── CommandeDAO.java
│   │   ├── ContientCommandeProduitDAO.java
│   │   └── FactureDAO.java
│   │   └── UtilisateurDAO.java
│   │	
│   ├── icon/                   ← Icons pour les interfaces
│   │
│   ├── service/               ← Logique métier
│   │   ├── ProduitService.java
│   │   ├── StockService.java
│   │   ├── CommandeService.java
│   │   └── FactureService.java
│   │   └── VenteService.java
│   │   └── ReportingService.java
│   │   └── UtilisateurService.java
│   │
│   ├── ui/                    ← Interface Swing
│   │   └── CommandeUI.java
│   │   └── VenteUI.java
│   │   └── Home.java
│   │   └── Login.java
│   │   └── FactureUI.java
│   │   └── Produit.java
│   │   └── CommandeUI.java
│   │
│   ├── util/                  ← Utilitaires généraux
│   │   └── DatabaseConnection.java
│   │   └── TestConnection.java
│   │
│   └── test/                  ← Tests unitaires JUnit 5
│       ├── ProduitServiceTest.java
│       └── CommandeServiceTest.java
│       └── StockServiceTest.java
│       └── VenteServiceTest.java
│
└── resources/                 ← Fichiers .txt
t…]()

✅ Fonctionnalités implémentées
Login

![Capture d'écran 2025-06-04 181034](https://github.com/user-attachments/assets/d1aab80d-2de6-4434-a6ba-c4869139ebc0)

Home/Dashbord

![Capture d'écran 2025-06-06 105223](https://github.com/user-attachments/assets/236f810d-224b-4236-8662-2346f99ba398)

Gestion des produits

![Capture d'écran 2025-06-04 182727](https://github.com/user-attachments/assets/18cbc61a-2503-400d-817a-4022da4d7619)

Gestion des commandes


Traitement des ventes

![Capture d'écran 2025-06-06 105041](https://github.com/user-attachments/assets/292ddf0e-f064-4bcc-a327-05ba8ade3669)

Génération de factures


Reporting quotidien


