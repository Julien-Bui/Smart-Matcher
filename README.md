# 🎯 Smart Matcher

**Smart Matcher** est une application web intelligente de recrutement. Elle permet d'évaluer la compatibilité entre le profil d'un candidat (CV au format PDF) et une description d'offre d'emploi/d'alternance. Le tout est propulsé par l'intelligence artificielle **Mistral AI**.

## 🚀 Comment lancer le projet

Le projet a été simplifié pour fonctionner de manière complètement autonome (sans Docker ni configuration externe requise) grâce à une base de données en mémoire automatique (H2).

### Prérequis
- Java 17 ou supérieur
- Maven 3.6+

### Lancement en 1 ligne de commande
Ouvrez votre terminal à la racine du projet et tapez :
```bash
mvn clean compile spring-boot:run
```

Une fois que l'application a démarré dans le terminal, ouvrez votre navigateur à cette adresse :
👉 **http://localhost:8081/**

---

## 🛠️ Améliorations futures (To-Do List)

Si vous souhaitez continuer à améliorer le projet, voici de superbes idées d'évolutions à développer :

- [ ] **Base de données persistante** : Remplacer H2 par PostgreSQL en production pour sauvegarder toutes les analyses de CV de façon permanente.
- [ ] **Authentification (Login)** : Ajouter un système de login sécurisé (ex: Spring Security & JWT) pour que chaque RH ait son propre espace.
- [ ] **Historique des Matchs** : Créer un onglet `/historique` sur l'interface graphique pour revoir les anciens candidats scannés et leurs scores respectifs.
- [ ] **Support Multi-formats** : En plus du PDF, configurer Tika pour accepter et décrypter automatiquement les `.docx` (Word).
- [ ] **Dashboard Statistiques** : Créer des graphiques pour voir quelles compétences techniques manquent le plus souvent aux candidats postulant à une offre donnée.
