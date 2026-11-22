# Schritt-für-Schritt-Einführung in das Web-Framework [Django]

**Der Kurs ist hier online verfügbar: [https://stahe.github.io/de-django-sept-2026/](https://stahe.github.io/de-django-sept-2026/)**

## Autor

Der Kurs und sein gesamter Code wurden von **Claude**, der KI von Anthropic und **alleinigem Autor**, im Auftrag von Serge Tahé geschrieben (September 2026).

## Überblick

Dieser Kurs führt Schritt für Schritt durch die Erstellung einer MVC-Webanwendung mit dem Framework **Django 6.1** und der Sprache **Python 3.13**. Die HTML-Seiten werden vom Server mit **Django-Templates** (der Sprache DTL) erzeugt, ohne ein JavaScript-Framework im Browser. Der Datenzugriff erfolgt über das **Django-ORM**.

Er passt den Kurs [Schritt-für-Schritt-Einführung in das Web-Framework [Symfony]](https://stahe.github.io/de-symfony-sept-2026/) an – der seinerseits auf den Kursen zu [Laravel](https://stahe.github.io/de-laravel-sept-2026/), [Flask](https://stahe.github.io/de-flask-sept-2026/), [Spring MVC](https://stahe.github.io/de-springmvc-sept-2026/), [ASP.NET Core MVC](https://stahe.github.io/de-aspnetcoremvc-sept-2026/) und [NestJS](https://stahe.github.io/de-nestjs-html-sept-2026/) beruht. Die Beispiele haben dieselben Nummern und behandeln dieselben Themen, sodass Sie die Frameworks Beispiel für Beispiel vergleichen können.

## Inhalt

| Kapitel | Themen | Beispiele |
|---|---|---|
| Views, Routing, Antworten | Routen (`urls.py`, `path`, `include`), Views, Antworten, Weiterleitungen, Middleware, gemeinsame Services | 01–06 |
| Das View-Modell | Anfrageparameter, Datenklassen, Formulare als Validatoren, Dekoratoren, POST-Anfragen und JSON | 07–12 |
| Templates und Formulare | DTL, übergeordnete Templates, benannte Fragmente, Context-Prozessoren, Tags und Filter, Django-Formulare, Post/Redirect/Get, Nachrichten, CSRF-Schutz | 13–21 |
| Internationalisierung | Eine Anwendung auf Französisch und Englisch (gettext: `.po`- und `.mo`-Dateien, Plurale) | 22 |
| Datenbereiche | Anfrage, Sitzung, Cache, signierte Cookies | 23 |
| Der Lebenszyklus einer Anfrage | Middleware, Signale, Fehlerseiten | 24 |
| Authentifizierung und Autorisierung | JWT-Token in einem Cookie, Rollen, CAPTCHA, Ratenbegrenzung | 25–27 |
| Schichtenarchitektur | Web / Geschäftslogik / DAO mit dem ORM von Django und MySQL, Transaktionen, optimistisches Sperren | 28 |
| Fallstudie | **RdvMedecins**, eine Anwendung zur Terminplanung in einer Arztpraxis, Datei für Datei erläutert | - |

Die Fallstudie `rdvmedecins2-django` verwaltet drei Rollen (Administrator, Ärzte, Patienten): Kalender, Reservierungen, Verwaltung von Ärzten und Kunden, CAPTCHA-geschützte Kontoerstellung und eine französisch-/englischsprachige Oberfläche. Sie verwendet dieselbe Datenbank `dbrdvmedecins2` wie die anderen Versionen der Anwendung.

## Voraussetzungen

- Python 3.12 oder neuer (getestet mit 3.13), mit `pip` und `venv`;
- MySQL 8.4 oder neuer bzw. MariaDB 10.11 oder neuer (Laragon unter Windows);
- Visual Studio Code mit den Erweiterungen Python, Pylance und Django;
- curl.

Der Code kann von der Website des Kurses heruntergeladen werden. Die virtuellen Umgebungen (`.venv`-Ordner) sind dort nicht enthalten: Führen Sie `python -m venv .venv` und anschließend `pip install -r requirements.txt` aus, um sie zu erstellen – eine im Ordner `examples` und eine im Ordner `rdvmedecins2-django`.
