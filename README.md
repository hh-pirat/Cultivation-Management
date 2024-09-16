Cultivation Management 1.1

Ein einfaches Tool zur Verwaltung und Dokumentation deines Pflanzen-Grows. Mit dieser Anwendung kannst du Pflanzen speichern, Ernteerinnerungen setzen und deine Gießprotokol übersichtlich darstellen.

Installation

    Datenbank einrichten:
        Erstelle eine MySQL-Datenbank mit dem Namen grow_diary.
        Importiere die Datei database.sql in deine MySQL-Datenbank, um die notwendigen Tabellen zu erstellen.

    bash

mysql -u [benutzername] -p [datenbankname] < path/to/database.sql

Konfiguration der Datenbankverbindung:

    Bearbeite die Datei config.php im Ordner config und trage deine Datenbankdetails ein:

    php

    $host = 'localhost';  // Datenbankhost
    $db = 'grow_diary';   // Datenbankname
    $user = 'grow';       // Benutzername
    $pass = 'password';   // Passwort

PHP Server starten:

    Du kannst den integrierten PHP-Server zum Testen verwenden:

    bash

        php -S localhost:8000

        Öffne deinen Browser und navigiere zu http://localhost:8000, um die Anwendung zu nutzen.

Funktionen

    Pflanzen hinzufügen: Gib den Namen der Pflanze, das Keimdatum und die Anzahl der Tage bis zur Ernte ein.

    Pflanzenübersicht: Eine Liste aller gespeicherten Pflanzen, einschließlich des Keimdatums und der verbleibenden Tage bis zur Ernte.

    Löschen von Pflanzen: Du kannst eine Pflanze löschen, indem du auf den Papierkorb klickst. Eine Bestätigung ist erforderlich.

    Automatisches Ausblenden von Meldungen: Erfolg- und Fehlermeldungen werden automatisch nach 3 Sekunden ausgeblendet.

Style

Das Design der Anwendung ist dunkel gehalten und verwendet einen einheitlichen Stil für alle Seiten.
Technologien

    Backend: PHP 7+
    Datenbank: MySQL
    Frontend: HTML, CSS, JavaScript

Lizenz

Dieses Projekt steht unter keiner spezifischen Lizenz und darf nach Belieben genutzt und verändert werden.
