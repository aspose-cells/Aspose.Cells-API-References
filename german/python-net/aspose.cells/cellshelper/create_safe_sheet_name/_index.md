---
title: create_safe_sheet_name Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 90
url: /de/python-net/aspose.cells/cellshelper/create_safe_sheet_name/
is_root: false
---
##  create_safe_sheet_name(name_proposal) {#str}
Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen.
Wenn der angegebene Blattname den Regeln des Excel-Blattnamens entspricht, geben Sie ihn zurück.
Andernfalls wird die Zeichenfolge abgeschnitten, wenn die Länge das Limit überschreitet
und ungültige Zeichen werden durch ' ' ersetzt, geben dann den neu erstellten Zeichenfolgenwert zurück.


###  Kehrt zurück




```python
def create_safe_sheet_name(self, name_proposal):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| name_proposal | str | Blattname, der verwendet werden soll|


##  create_safe_sheet_name(name_proposal, replace_char) {#str-char}
Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen.
Wenn der angegebene Blattname den Regeln des Excel-Blattnamens entspricht, geben Sie ihn zurück.
Andernfalls wird die Zeichenfolge abgeschnitten, wenn die Länge das Limit überschreitet
und ungültige Zeichen werden durch das angegebene Zeichen ersetzt und geben dann den neu erstellten Zeichenfolgenwert zurück.


###  Kehrt zurück




```python
def create_safe_sheet_name(self, name_proposal, replace_char):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| name_proposal | str | Blattname, der verwendet werden soll|
| replace_char | char | Zeichen, das verwendet wird, um ungültige Zeichen im angegebenen Blattnamen zu ersetzen|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [CellsHelper](/cells/de/python-net/aspose.cells/cellshelper)
