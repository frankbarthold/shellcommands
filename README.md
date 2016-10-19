# shellcommands

\# Mac OS // Linux

\# Herausfinden, ob und von welchem Prozess ein Port belegt ist
>lsof -i :8080

\# oder mit netstat ohne Prozessinfo
>netstat -a | grep LISTEN

\# PHP Built-in-server starten
\# Für Frameworks wie ZF2, muss vorher ins public Verzeichnis gewechselt werden
>cd path/to/project/*public*/
>php -S localhost:5080 index.php

\# ORM Schema Helferfunktionen 

\# Ins Vendor-Bin-Vzs. wechseln, um direkt das Shell-Script aufzurufen
>cd path/to/project/vendor/bin/

\# ORM-Mapping validieren
>path/to/project/vendor/bin/doctrine-module orm:validate-schema

\# Datenbank anlegen lassen
>path/to/project/vendor/bin/doctrine-module orm:schema-tool:create
