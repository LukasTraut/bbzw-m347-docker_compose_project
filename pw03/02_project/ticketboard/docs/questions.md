# Fragen – Konfiguration und Umgebungsvariablen (DL11)

Name: <Nachname> <Vorname>
Klasse: <Klasse>

---

## 1. Konfiguration

Welche Werte waren ursprünglich hardcoded in `compose.yml` und `app/main.py`?

Antwort:

Database url und Postgres sachen

Warum ist es ein Problem, Passwörter direkt in `compose.yml` einzutragen?

Antwort:

es bleibt in der History des git Repos

Was ist der Unterschied zwischen `.env` und `.env.example`?

Antwort:

.env sind echte dtaen und example testdaten

Warum muss `.env` in `.gitignore` eingetragen sein?

Antwort:

weil in .env echte daten sind

## 2. Variablen in Compose

Wie referenziert man eine Variable aus `.env` in `compose.yml`?

Antwort:

per syntax

Was passiert, wenn eine Variable in `.env` fehlt, aber in `compose.yml` verwendet wird?

Antwort:

es werden wahnungen ausgegeben

Was zeigt der Befehl `docker compose config`? Wann ist er nützlich?

Antwort:

---

## 3. Dockerfile und Build

Warum wird `requirements.txt` in einem eigenen `COPY`-Schritt vor dem App-Code kopiert?

Antwort:

wegen den Layer von den Docker

Was bewirkt `.dockerignore`? Welche Dateien sollten darin stehen?

Antwort:

es wird beim aufstarten von einem Docker Container ignoriert

## 4. Systemtest

Funktioniert `/db-check` nach Ihrer Konfigurationsanpassung?

Antwort:

ja

Was zeigt der Endpunkt `/db-check` an, wenn die Verbindung funktioniert?

Antwort:

```json
{"db": "connected"}
```

## 5. Reflexion

Was war der wichtigste Schritt in dieser Woche?

Antwort:

zu verstehen was der Unterschied der verschiedenen .env dateien ist

Was ist noch unklar oder möchten Sie besser verstehen?

Antwort:
