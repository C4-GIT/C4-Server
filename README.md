# C4-Server Umgebung
![tower-31235_960_720-645792324](https://github.com/user-attachments/assets/d270746b-56af-40b1-ae0f-c16a5bb5d42e)

# Übersicht C4-Server
Einfacher Script, welcher unterschiedliche Server startet und den Zugriff auf die C4-Anwendungen bereit stellt. Über diese Verbindungen sollten Daten von z.B dem C4-Terminal Script an den C&C Server übertragen werden und die Persistens der Agententen erfolgen. Zu Beginn sollte ein http/https Server installiert werden und gestartet werden können. Des Weiteren, sollten der Proxy-Server gestartet werden nachdem dieser Installiert wurde. Die wichtigsten Funktionen sind die Kommunikation mit den Agenten, sowie aller C4-Software Komponenten. Die Agenten können sich nach dem Start der sysget Datei an dem C&C-Server anmelden und die ersten Informationen übertragen. Die C4-Server Anwendung sollte auch das einrichten eines Dienstes automatisch ausführen und starten. 

- HTTP/HTTPS Server
- FTP/FTPS Server
- MySQL/SQLite-Server 
- Proxy/Reverse-Proxy-Server
- Onion-Share

Die Verschiedenen Server werden mittels c4_server.py gestartet, wenn sie noch nicht installiert sind. Es sollte wieder eine Terminal Version und eine GUI-Anwendung vorhanden sein, um die Server Verknüpfungen zu erstellen und Verwalten. 

# C4-Server Initialisierung
### Automatische Server installation und Bereitschaft. 
- Lokal
- Remote



### Start der Installation. 
- sudo apt update -y
- sudo apt full-upgrade -y

## C4-Server Starten
- Verbindungen
- Webserver
- Datenbank
- 


### Terminal 
Mit dem Punkt 2 in der Auswahl, kann die Umgebung gestartet werden. 

Über der IP-ADRESSE/Hostname:5000 kann mittels Browser auf die C4-WebAnwendungen zugegriffen werden. 

### Python Anwendung
Python Anwendung mit GUI, welche die ganze C4-Umgebung mittels Button starten und stoppen kann, aber auch die einzelnen Server komponenten. Die Verschlüsselung soll mittels Import und Export von Zertifikaten ermöglicht werden, und durch config Dateien der aufbau von Tunneln zu Remote-Systemen. 

# Der C4-Webserver
![himars](https://github.com/user-attachments/assets/c3189d09-1f51-45c9-a05b-7c4cc95982ab)
Der C4-Webserver dient als grafische Schnittstelle zur C4-Server Umgebung. Die Webseiten sind unterteilt in die folgenden Bereiche:
## Startseite
### webserver.html
Bestehend aus Logo, Überschrift, Zusammenfassung der Übersicht, Menü und ganz wichtig, einer Übersicht der Statistiken aus der C4-Umgebung.

## Agenten & Hosts
### agents-hosts.html
Auflistung und Steuerung der Agenten soll die Remote-Administration ermöglichen und erleichtern.

## C4-Krypto
### c4-crypto.html
Ein Teil der C4-Krypto Umgebung ist die Ver/Entschlüsselung, Codierung. Ein anderer ist die Transaktions-Verwaltung, Lagerung von Elektronischen Geldmitteln, sowie der Überweisung. Ziel ist die Verwaltung der Geschäftsprozesse, inbegriffen die Verwaltung der Kunden in Bezug Sicherer Kommunikation zur Remote-Administration, Sicherer Austausch von Informationen und Daten. 
