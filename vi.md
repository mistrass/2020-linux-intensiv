## 14 vi 

### vimtutor 

```
# Interactives Tutorial zum Lernen von vi 
# Wichtigste Befehle 
vimtutor # sollte bereits mit vi installiert worden sein.
```

### Wichtigste Aktionen 

```
  1. # Öffnen eine neuer Datei mit vi 
  vi dateiname 
  
  2. # Schreiben in der Datei 
  i # drücken
  
  3. # Es erscheint unten in der Zeile 
  # -- INSERT -- 
  
  4. # Nun können Sie etwas hineinschreiben 
  
  5a. Beenden ohne Speichern (wenn geänderter Inhalt vorhanden ist  
  ESC + :q! # ESC Taste drücken, dann : und q! und enter 
  
  5b. Oder: Speichern und schliessen 
  ESC + :x # ESC Taste drücken, dann : und w und enter 
```  

### Virtual Mode 

```
v Zeichenweise markieren einschalten
V Zeilenweise markieren einschalten
STRG + v Blockweise markieren 

# mit Cursortasten auswählen / markieren 
# Dann:
x # Löschen des markierten Bereichs 
```

### Zeilen löschen im Normalmodus (Interactiver Modus) 

```
ESC + dd # eine Zeile löschen 
# letzte Aktion rückgängig machen 
ESC + u # eigentlich reicht 1x Escape 
# mehrere Zeilen löschen z.B. 1000
ESC + 1000dd # ESC - Taste drücken, dann 1000 eingeben, dann dd (sie sehen die 1000 nicht auf dem Bildschirm) 
```
