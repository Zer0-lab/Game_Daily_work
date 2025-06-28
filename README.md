Pour que le projet démarre il faut: 
- Changer dans le .env:
  - UID et le GID par celui correspondant à votre machine
  - DB_HOST par mysql

Pour récupérer l’UID et le GUID sur un PC

Linux / macOS

Récupérer l’UID (User ID)

id -u

Récupérer le GUID / GID (Group ID)

id -g

Pour afficher toutes les informations d’identité :

id

Affiche UID, GID et les groupes supplémentaires de l’utilisateur.

⸻

Windows

Windows n’utilise pas directement UID/GID, mais des SID (Security Identifiers) pour identifier les utilisateurs et groupes.

Récupérer le SID avec PowerShell

Liste tous les utilisateurs locaux avec leur SID :

Get-LocalUser | Select Name, SID

Récupérer le SID d’un utilisateur spécifique :

(Get-LocalUser -Name "NomUtilisateur").SID

Utilise ces commandes dans un terminal (Linux/macOS) ou PowerShell (Windows).
