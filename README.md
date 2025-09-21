# Langflow Docker Compose Setup 🚀

## Übersicht 🌟
Willkommen! Dieses Dokument bietet eine einfache Anleitung zur Verwendung der Docker Compose-Konfiguration für die Installation einer Langflow-Instanz. Hier finden Sie alles, was Sie benötigen, um schnell loszulegen!

## Voraussetzungen 📋
- **Docker**: [Installationsanleitung hier](https://docs.docker.com/get-docker/)
- **Docker Compose**: [Installationsanleitung hier](https://docs.docker.com/compose/install/)

## Nutzung 🛠️
1. **Überprüfen Sie, ob Docker und Docker Compose installiert sind**.
2. **Navigieren Sie zum Verzeichnis** mit der `docker-compose.yml`-Datei.
3. **Starten Sie den Dienst** mit folgendem Befehl:
   ```bash
   docker-compose up -d
   ```
4. **Zugriff auf die Langflow-Anwendung**: Besuchen Sie [http://localhost:7860](http://localhost:7860) in Ihrem Webbrowser.

5. **Um den Dienst zu stoppen**, verwenden Sie:
```bash
docker-compose down
```

## Volumes 🗂️
- **Files Volume**: `./files:/app/files` (Dieses Volume dient dazu, Dokumente und Dateien an Langflow weiterzugeben, um den Modul Directory nutzen zu können. Es ermöglicht Ihnen, Dateien zwischen Container-Läufen zu persistieren und sicherzustellen, dass Langflow auf benötigte Ressourcen zugreifen kann. Bitte stellen Sie sicher, dass Sie das `./files`-Verzeichnis manuell erstellen, da es sonst automatisch generiert wird.)
