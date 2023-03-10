---
title: find_formula Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 300
url: /de/python-net/aspose.cells/cells/find_formula/
is_root: false
---
##  find_formula(formula, previous_cell) {#str-Cell}
Findet die Zelle mit der Eingabezeichenfolge.


###  Kehrt zurück

Cell Objekt.


```python
def find_formula(self, formula, previous_cell):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| formula | str | Die zu suchende Formel.|
| previous_cell | [Cell](/cells/de/python-net/aspose.cells/cell) |Vorherige Zelle mit derselben Formel. Dieser Parameter kann auf null gesetzt werden, wenn von Anfang an gesucht wird.|
###  Bemerkungen

Gibt null (Nichts) zurück, wenn keine Zelle gefunden wird.
 HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen,
Bitte verwenden Sie die Methode Cells.Find(object,Cell,FindOptions) mit LookInType als LookInType.OnlyFormulas
 und LookAtType als LookAtType.EntireContent.
 Dieses Mitglied wird 12 Monate später seit November 2018 entfernt.
Aspose entschuldigt sich für etwaige Unannehmlichkeiten.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cells](/cells/de/python-net/aspose.cells/cells)
