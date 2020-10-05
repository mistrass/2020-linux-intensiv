# Linux Einführung 

## Wann Linux, wann Windows ? 

https://www.computerweekly.com/de/meinung/Das-beste-Server-Betriebssystem-Vergleich-zwischen-Linux-und-Windows#:~:text=Linux%20kommt%20im%20Data%20Center,viele%20verschiedene%20Einsatzzwecke%20zu%20verwenden.

## Bash Specials 

```
# Zeigt Heimatverzeichnis des aktuell eingeloggten Nutzers an 
echo ~
# Ausgeführte Befehle während meiner Session 
history 
# Bestimmten Befehl aus der History ausführen:
# !nr 
# Beispiel 
!244  # Achtung wird direkt ausführt 
```


## Verzeichnis wechseln und Liste anzeigen 
```
# Verzeichnis wechseln 
cd /

# In das Heimat oder User-Verzeichnis wechseln
cd

# Ein Verzeichnis höher wechseln 
cd ..

# Verzeichnis anzeigen, in dem ich bin 
pwd 

# Verzeichnisliste anzeigen 
ls -l 

# Liste mit versteckten Dateien 
ls -la

# Listing seitenweise anzeigen (Pager) 
ls -la  | less 

```

## Verzeichnis anlegen, löschen und umbenennen 

```

# mit relativem Pfad / im aktuellen Verzeichnis 
mkdir training  
mkdir /home/user/training2 

# Verzeichnisstruktur anlegen (-p)  
mkdir -p daten/2020/dezember 

```
## Hintergrund '.' und '..' 
. = aktuelles Verzeichnis 
.. = übergeordnetes Verzeichnis 

ls -la training
total 8
drwxrwxr-x  2 nobleprog nobleprog 4096 Oct  5 09:22 .
drwxr-xr-x 24 nobleprog nobleprog 4096 Oct  5 09:22 ..
```


```
# Leeres Verzeichnis löschen 
rmdir verzeichnisname 


## Datei anlegen/löschen  

```
# Anlegen 
touch dateiname

# Löschen mit Nachfrage 
rm -i dateiname 

# Löschen ohne Nachfrage 
rm dateiname 

# Ausgabe - keine Berechtigung 
nobleprog@jochen-g14d:/$ rm vmlinuz.old 
rm: cannot remove 'vmlinuz.old': Permission denied

# Löschen von Verzeichnissen
rm -r verzeichnis 
rm -R verzeichnis 

```

## Hilfe ## 

```
man ls 
# (Verlassen mit q )

### Suchen in der Hilfe 
/suchbegriff + Enter 
# nächster Vorkommen Taste ->  
n (wie next) 

# hilfeseite des man - kommandos 
man man 


befehl --help 
oder 
befehl -h 

Beispiel:
ls --help 

```

## Benutzer ##

```
# Wer bin ich / Unter welchem Benutzer bin ich eingeloggt  
whoami 

# Mehr über mich
id
```
