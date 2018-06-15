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

\# NPM Update
>npm install -g npm


\# Make Git-Bash available in CMD Commandline Prompt via bat-Script

\# Create git-bash.bat and this Script to your PATH-Env-Var
@echo off

REM "FIT Your Path to sh.exe in yout git-bash program-folder

IF [%1]==[] (

REM "WithOut Args, open git-bash-terminal"    

    C:\WINDOWS\system32\cmd.exe /c ""C:\Users\f.barthold\AppData\Local\Programs\Git\bin\sh.exe" --login -i"
    
) ELSE (

REM "WithArgs, execute git-bash with Args using -c Option"

    C:\WINDOWS\system32\cmd.exe /c ""C:\Users\f.barthold\AppData\Local\Programs\Git\bin\sh.exe" --login -i -c %*"
    
)

