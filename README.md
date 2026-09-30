# Site CV - rahul.local

## Installation
- sudo apt install apache2
- Dossier du site : /var/www/html/rahul (index.html)

## Configuration Apache
Fichier /etc/apache2/sites-available/rahul.local.conf :
<VirtualHost *:80>
    ServerName rahul.local
    DocumentRoot /var/www/html/rahul
</VirtualHost>

Activation : sudo a2ensite rahul.local.conf && sudo systemctl reload apache2

## Nom de domaine local
Ligne ajoutée dans /etc/hosts : 127.0.0.1 rahul.local

## Test
curl http://rahul.local
