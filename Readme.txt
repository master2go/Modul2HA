In einem neuen Projekt muss folgendes gemacht werden:
  1. Alles ausser .git kopieren
  2. In dem entstanden Ordner dann die Dateien im Ordner Stoff löschen
  3. Neue unter Stoff erstellen und darauf achten die Dateien zu nummerieren
  3a. Unter Titel die Titeldatei ändern
  4. Nun im makefile unter TARGET die neue Zieldatei benennen
      (man könnte den Namen auch so lassen, aber dann heißen halt Dateien gleich)
  5. Auf github ein neues Rep z.b. mit dem Namen: Modul2HA erstellen
  6. Im Terminal dann folgende Befehle:
  git remote add origin https://github.com/master2go/Modul2HA.git
  git init
  git add .
  git commit -m 'Initial Commit'
  git push -u origin master


  7. Im weiteren Verlauf des Schaffens jetz einfach immer wieder mit dem Befehl:
  git commit -a
 git push
  alles ins entfernte Rep übertragen
  8. Falls neue Dateien hinzukommen:
   git add .

   Wenn das alles steht ist es Kinderleicht:
    1. Atom öffen, New file, Speichern unter dem eben erstellten Projekt unter /Stoff nummerierten Namen mit Dateiendung .md
    2. Das wichtigste ist natürlich: Denken und Schreiben und Zitieren...
    3. im Terminal make eingeben und alles passiert wie von Geisterhand :)
    4. git commit -m "Text" und git push (bzw. git add .) schafft alles ins entfernte Rep
    5. entspannt zurücklehnen, alles ist safe...
    6. Ändert man unterwegs etwas z.B. mit workcopy auf dem iPad pusht man es von dort und gibt zuhause einmal git pull
    dann das ist das lokale wieder auf dem Stand
