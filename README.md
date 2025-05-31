# Active-Directory-Project

📌 Ziel dieses Projekts
In diesem Tutorial erstellen wir eine automatisierte Sicherheitsumgebung mit Active Directory (AD), Splunk, Shuffle und Slack, um Angriffe zu erkennen und automatisiert darauf zu reagieren. Ziel ist es, nicht nur eine realistische Angriffs- und Verteidigungsumgebung zu bauen, sondern auch Troubleshooting-Fähigkeiten zu schärfen und Security-Automation hands-on zu erleben.

🧠 Projektüberblick
Ein externer Angreifer (simuliert durch eine Angriffsmaschine im Internet) scannt und greift ein Windows-Testsystem an. Gelingt die Authentifizierung (z. B. durch gültige Zugangsdaten), wird dieses Ereignis über Telemetriedaten an Splunk gemeldet. Dort wird eine Alarmregel ausgelöst, die:

eine Benachrichtigung an Slack sendet,

ein Playbook in Shuffle startet.

Dieses Playbook fragt automatisiert beim SOC-Analysten (per E-Mail) nach, ob der kompromittierte Benutzer deaktiviert werden soll. Bestätigt der Analyst, wird der Benutzeraccount im AD deaktiviert und eine Benachrichtigung über den Vorgang an Slack gesendet.

🔧 Verwendete Tools & Ressourcen
Visualisierung: Draw.io (Logisches Diagramm)

Cloud-Infrastruktur: Vultr (300 $ Credit)

SIEM: Splunk

Security Automation: Shuffle

Kommunikation & Benachrichtigungen: Slack

Directory Services: Active Directory

📚 Tutorialstruktur
🧩 Teil 1: Logisches Architekturdiagramm erstellen
Erstellung eines logischen Netzwerkdiagramms zur besseren Planung und Dokumentation der Umgebung mit Draw.io.

☁️ Teil 2: Cloud-Umgebung einrichten (Vultr)
Deployment der Infrastrukturkomponenten auf Vultr mit Hilfe des Cloud-Guthabens.

🛠️ Teil 3: Active Directory installieren & konfigurieren
Installation eines Windows Servers, Einrichtung von AD Domain Services und Vorbereitung für spätere Automatisierungsschritte.

📊 Teil 4: Splunk konfigurieren & Alarme einrichten
Einrichtung von Splunk zur Erfassung von Windows-Telemetriedaten und Definition von Alert-Regeln auf sicherheitsrelevante Ereignisse.

🤖 Teil 5: Integration von Slack & Shuffle zur Automatisierung
Anbindung von Slack zur Alarmierung und Aufbau eines automatisierten Incident-Response-Prozesses via Shuffle.

🎯 Lernziele
Verständnis für SIEM-Integration mit AD

Einführung in Security Automation mit Shuffle

Troubleshooting realitätsnaher Angriffsszenarien

Umsetzung von Detection-to-Response-Ketten in Echtzeit

![AD_Project_Diagram drawio](https://github.com/user-attachments/assets/dcb8714a-391f-462e-b079-2bfbf855d261)

