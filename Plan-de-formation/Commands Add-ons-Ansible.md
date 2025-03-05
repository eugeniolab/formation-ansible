# Comment configurer l'authentification sans mot de passe pour les instances EC2

## Utilisation de la clé publique

La commande suivante permet de copier votre clé publique sur une machine distante :

```bash
ssh-copy-id -f "-o IdentityFile <CHEMIN VERS LE FICHIER PEM>" ubuntu@<IP-PUBLIQUE-DE-L'INSTANCE>
