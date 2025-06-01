Cahier des Charges - Système de Gestion de Cabinet Médical Multi-praticiens
1. Présentation Générale du Projet
1.1 Contexte
La gestion des cabinets médicaux multi-praticiens s’effectue encore souvent à l’aide d’outils hétérogènes. Ce projet vise à digitaliser et centraliser tous les processus métier spécifiques à ce type de structure, tout en respectant les réglementations sanitaires et les standards de sécurité.
1.2 Objectifs
- Centraliser la gestion du cabinet dans un système unique et sécurisé.
- Optimiser la planification des rendez-vous et la facturation.
- Intégrer les normes médicales françaises (CCAM, CIM-10, SESAM-Vitale).
- Assurer la confidentialité des données de santé conformément au RGPD.
- Permettre un suivi comptable médical spécialisé.
2. Acteurs du Système
Acteur	Rôle
Praticien	Gère ses patients, prescrit, facture, consulte les dossiers médicaux.
Secrétaire	Planifie les RDV, gère les patients et les créneaux de plusieurs praticiens.
Patient	Consulte son dossier, prend rendez-vous, reçoit ses ordonnances.
Administrateur	Supervise le système, configure les accès, consulte les statistiques globales.
3. Fonctionnalités Fonctionnelles
3.1 Gestion des utilisateurs
- Authentification sécurisée
- Rôles
- Chiffrement des mots de passe
3.2 Agenda médical
- Calendrier par praticien
- Vue hebdomadaire/journalière
- Créneaux dynamiques
- Notifications
3.3 Dossier patient
- Fiche complète
- Historique des consultations
- Upload de documents
3.4 Facturation médicale
- Génération de factures
- Intégration des mutuelles
- Calcul automatique selon CCAM
3.5 Télétransmission simulée
- Génération de FSE
- Envoi vers API simulée
3.6 Comptabilité médicale
- Export BNC
- Gestion des amortissements
- Suivi des paiements
3.7 Statistiques médicales
- Taux de fréquentation
- Répartition par pathologie
- Taux d’absentéisme
4. Exigences Techniques
Élément	Détails
Backend	Spring Boot 3.2, Spring Security, JPA, Spring Integration
Frontend	React 18, TypeScript, Shadcn, FullCalendar
Base de données	MySQL avec chiffrement des données sensibles
API externes	Télétransmission simulée, base médicamenteuse
Chiffrement	AES/PGP pour les données sensibles
Audit	Historique des actions critiques
Conformité	RGPD, confidentialité médicale, consentement patient
5. Modèle de Données (Extrait simplifié)
Tables principales
Table	Champs
Utilisateur	id, nom, rôle, email, mot_de_passe
Patient	id, infos personnelles, antécédents
RendezVous	id, date, heure, praticien_id, patient_id
Facture	id, patient_id, montant, statut, mutuelle
Prescription	id, consultation_id, médicaments, posologie
DossierMedical	id, patient_id, consultations, fichiers
6. Architecture Logicielle
- Backend REST API avec Spring Boot
- Frontend SPA avec React et Ant Design
- Communication HTTP sécurisée via JWT
- Architecture MVC + DAO/Service pour la couche métier
7. Sécurité
- Authentification & autorisation via Spring Security
- Stockage des mots de passe en BCrypt
- Chiffrement AES des données médicales
- Audit trail des actions
- Accès différenciés par rôle (RBAC)
8. Planning prévisionnel
Période	Tâches
Semaine 1-2	Analyse des besoins, rédaction cahier des charges
Semaine 3-4	Conception base de données, maquettage UI
Semaine 5-6	Développement backend
Semaine 7-8	Développement frontend
Semaine 9	Sécurité, tests fonctionnels
Semaine 10	Rédaction du rapport, soutenance
9. Livrables attendus
- Application Web fonctionnelle
- Rapport de PFE complet
- Documentation technique
- Présentation de soutenance avec démonstration
