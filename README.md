# docker_httpd_WA
Petite serveur WEB pour tester en vitesse une map de Work Adventure sur sa machine au lieu de sur GitHub pages
zf210308.1611

Juste un petit container avec un serveur web Apache ;-)


## Configuration
Il faut modifier la ligne:
```
/Users/zuzu/dev-vpsi/WA-INN:/usr/local/apache2/htdocs/
```
dans le fichier docker-compose.yml en indiquant son path (/Users/zuzu/dev-vpsi/WA-INN) où se trouve WA !


## Utilisation 
Pour le démarrer, simplement faire:
```
./start.sh
```

Pour l'arrêter, faire:
```
./stop.sh
```

Pour utiliser Work Adventure sur sa machine il faut systématiquement ouvrir WA dans une fenêtre de navigation privée, autrement on risque de ne pas voir ses dernières modifications !

Faut le faire AVEC Firefox, car Chrome n'aime pas les certificats auto-signés:

https://localhost


# Remarques:
Si on veut absolument utiliser le browser Chrome, il faut quand on se trouve dans la zone 'dangereuse' tapper au clavier:

thisisunsafe

Après, cela débloque Chrome et on peut l'utiliser


# Goodies

Pour refaire un certificat SSL auto-signé:
```
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout server.key -out server.crt
```




