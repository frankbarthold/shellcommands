# shellcommands

\# Mac OS // Linux

\# Herausfinden, ob und von welchem Prozess ein Port belegt ist
>lsof -i :8080

\# oder mit netstat ohne Prozessinfo
>netstat -a | grep LISTEN

\# PHP Built-in-server starten
\# Für Frameworks wie ZF2, muss vorher ins public Verzeichnis gewechselt werden
>cd path/to/zf/project/folder/public/
>php -S localhost:5080 index.php
