---
title: set_footer Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 180
url: /de/python-net/aspose.cells/pagesetup/set_footer/
is_root: false
---
##  set_footer(section, footer_script) {#int-str}
Legt ein Skript fest, das die Fußzeile einer Excel-Datei formatiert.



```python
def set_footer(self, section, footer_script):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| section | int | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt.|
| footer_script | str | Skript für das Fußzeilenformat.|
###  Bemerkungen

Skriptbefehle:

| Befehl| Beschreibung|
| :- | :- |
| &P| Aktuelle Seitenzahl|
| &N| Seitenzahl|
| &D| Aktuelles Datum|
| &T| Aktuelle Uhrzeit|
| &A| Blattname|
| &F| Dateiname ohne Pfad|
| &"<FontName>"| Schriftartname, zum Beispiel: &"Arial"|
| &"<FontName>, <FontStyle>"| Schriftname und Schriftstil, zum Beispiel: &"Arial,Bold"|
| &<FontSize>| Schriftgröße. Folgt diesem Befehl eine einfache Zahl, die in der Kopfzeile ausgegeben werden soll, wird diese durch ein Leerzeichen von der Schrifthöhe getrennt.|
| &K<RRGGBB>|Schriftfarbe, zum Beispiel (ROT): &KFF0000|
| &G| Bildskript|

Zum Beispiel: „&Arial,Bold&8Footer Note“


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [PageSetup](/cells/de/python-net/aspose.cells/pagesetup)
