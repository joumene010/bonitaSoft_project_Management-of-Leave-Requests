📋 Gestion des Demandes de Congés avec Bonitasoft
Bonitasoft Workflow Demo

📌 Aperçu du Projet
Ce projet vise à automatiser la gestion des demandes de congés dans une entreprise en utilisant Bonitasoft, un outil de gestion de processus métier (BPM). Le système permet aux employés de soumettre des demandes, aux superviseurs de les valider, et notifie toutes les parties concernées par e-mail.

✅ Fonctionnalités Principales
Soumission des demandes via une interface intuitive.

Validation hiérarchique automatisée (employé → reporter → manager).

Notifications par e-mail pour les acceptations/refus.

Transparence et traçabilité grâce à un workflow clair.

📊 Workflow du Processus
Soumission : L’employé remplit un formulaire de demande.

Révision :

Le reporter vérifie la demande.

Le manager approuve ou refuse.

Notification :

Acceptation → e-mail de confirmation.

Refus → e-mail avec motifs.

Diagramme BPMN
BPMN Diagram

⚙️ Configuration Technique
Acteurs & Rôles
Groupe	Rôle	Responsabilité
Employees	Requester	Soumettre une demande
Supervisors	Reporter	Vérifier la demande
Reporter	Manager/HR	Valider ou refuser
Connecteurs Utilisés
SMTP pour les notifications (ex: localhost:25).

Base de données métier pour stocker les demandes.

🚀 Installation & Utilisation
1. Prérequis
Bonita Studio (version 7.x ou supérieure).

Serveur SMTP local (ex: FakeSMTP pour les tests).

2. Importer le Projet
Ouvrir Bonita Studio.

Importer le fichier .bos (disponible dans /bonita-export).

3. Configurer les Connecteurs
SMTP :

Copy
Host: localhost  
Port: 25  
From: ${requester.email}  
Base de données : Modifier les paramètres dans Business Data.

4. Exécuter le Processus
Lancer le Bonita Runtime.

Se connecter en tant qu’employé/superviseur via l’interface web.

📸 Captures d’Écran
Étape	Image
Soumission	Form
Validation Manager	Approval
Notification (FakeSMTP)	Email
📈 Avantages
✔ Réduction des erreurs via l’automatisation.
✔ Gain de temps pour les RH et les managers.
✔ Historique centralisé des demandes.
