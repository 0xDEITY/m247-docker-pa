# M247 Apache2 Webserver mit Docker

![Preview](https://cdn.discordapp.com/attachments/714785316594122793/1109916743322837052/image.png)

## Installation
- Repository herunterladen und entzippen
- Das Image builden: `docker build -t m247-apache-dp .`

## Start
- Image entwicklungsbereit starten (Port 8080): `docker run -dit --name m247-apache-dp-seite -v $(pwd):/usr/local/apache2/htdocs -p 8080:80 m247-apache-dp`

## Hilfe

### Wieso `$(pwd)` beim Start des Containers?
Es wird ein Mount direkt in der momentanen Directory erstellt, damit kann man direkt Änderungen auf die index.html Datei vornehmen, und sie werden direkt sichtbar.

## Ressourcen / Referenzen

- https://hub.docker.com/_/httpd
- https://www.freecodecamp.org/news/docker-mount-volume-guide-how-to-mount-a-local-directory/
- Schulmaterial

`Dalibor`
`Pascal`
