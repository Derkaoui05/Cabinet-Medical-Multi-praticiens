# Projet : Système de Gestion de Cabinet Médical Multi-praticiens

## Description
Une plateforme complète de gestion pour les cabinets médicaux multi-praticiens, offrant des modules pour la gestion des agendas, dossiers patients, facturation, télétransmission, et comptabilité médicale.

## Problématique 
Digitaliser la gestion de cabinets médicaux avec des spécificités métier complexes incluant la nomenclature médicale, la télétransmission sécurisée et la gestion comptable spécialisée.

## Stack Technique

### Backend
- Spring Boot 3.2
- Spring Security
- Spring Data JPA
- Spring Integration

### Frontend
- React 18, react-router
- TypeScript
- FullCalendar
- Shadcn

### Base de données
- MySQL avec chiffrement des données sensibles

### Sécurité
- Conformité RGPD
- Chiffrement
- Audit trails

### Intégration
- APIs de télétransmission (simulées)

### Calculs financiers
- Nomenclature médicale (CCAM, dépassements d’honoraires)

## Fonctionnalités techniques avancées

- Système d'agenda médical avec gestion complexe des créneaux
- Module de télétransmission avec formatage SESAM-Vitale
- Calcul automatique des actes médicaux selon nomenclature CCAM
- Dossier médical complet et historisé
- Facturation avec gestion du tiers-payant et des mutuelles
- Comptabilité médicale (BNC, amortissements de matériel médical)
- Système de rappels automatiques et gestion des rendez-vous ratés
- Statistiques médicales respectant l’anonymat

## Spécificités médicales

- Respect strict de la confidentialité médicale
- Intégration des nomenclatures françaises (CCAM, CIM-10)
- Gestion des prescriptions avec base médicamenteuse
- Workflows de validation médicale

## Auteur
Derkaoui Yassir
