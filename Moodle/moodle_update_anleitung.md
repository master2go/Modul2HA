### Moodle-Update-howto

* Alles sichern und zwar so:

1. ssh username@master2go.de

2. cp -r moodle-data ./backup

3. cp -r moodle ./backup

4. Datenbank sichern:
cd backup
mysqldump -h  -u=dbusw.  --password=geheim -C -Q -e --create-options dbusw > moodle-database.sql

5. Seite in den Wartungsmodus:
Als Administrator/in können Sie auf der Seite Einstellungen > Website-Administration > Server > Wartungsmodus den Wartungsmodus aktivieren.
Im Textbereich Wartungsinformationen können Sie eine eigene Meldung eintragen.
Wenn Ihre Moodle-Site im Wartungsmodus ist, wird ein entsprechender Link rechts oben auf der Seite angezeigt.

6. neue Software holen:
 wget http://sourceforge.net/projects/moodle/files/Moodle/stable30/moodle-latest-30.tgz

7. mv moodle moodle.backup (das ist eigentlich nicht notwendig, denn das backup wurde ja schon gemacht)
8. tar xvzf moodle-latest-30.tgz
9. Jetzt müssen Sie noch den eignetlichen Aktualisierungsprozess in Moodle anstoßen. Gehen Sie dazu auf die Seite Einstellungen > Website-Administration > Mitteilungen.
Moodle erkennt automatisch, dass eine neuere Version auf den Server hochgeladen wurde und startet die Aktualisierung der Moodle-Datenbank und des Moodle-Datenverzeichnisses. Wenn irgendetwas nicht automatisch aktualisiert werden kann, sehen Sie entsprechende Hinweise und Anleitungen, was Sie tun sollen.
Wenn alles erfolgreich und ohne Fehlermeldungen durchläuft, dann können Sie mit Ihrer neuen Moodle-Version sofort loslegen!


Siehe auch:
https://www.youtube.com/watch?v=k5rwTy3sNh0
https://docs.moodle.org/27/de/Aktualisierung_von_Moodle

Und das ganze auch auf dem localhost durchführen und zwar hier:
/Applications/MAMP/htdocs
es funktioniert so ziemlich gleich
