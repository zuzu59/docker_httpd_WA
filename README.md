# docker_httpd_WA
Petite serveur WEB pour tester en vitesse une map de Work Adventure sur sa machine au lieu de sur GitHub pages
zf210308.1600

Juste un petit container avec le serveur web Apache ;-)


## Utilisation 
Pour le démarrer, simplement faire:
```
./start.sh
```

Pour l'arrêter, faire:
```
./stop.sh
```

Pour utiliser Work Adventure sur sa machine il faut faire AVEC Firefox (car Chrome n'aime pas les certificats auto-signés):

https://localhost




## ATTENTION


ATTENTION, ce n'est plus valable ! zf210308.1355
Cette version de déploiement n'exporte PAS le port 80 du serveur web lighttpd !<br>
Le port 80 de lighttpd est utilisable seulement depuis l'intérieur du réseau Docker, il faut donc l'utiliser par exemple avec reverse proxy traefik pour exporter CE serveur web lighttpd !









