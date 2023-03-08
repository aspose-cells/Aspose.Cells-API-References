---
title: trim_leading_blank_row_and_column Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 220
url: /de/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column/
is_root: false
---
##  trim_leading_blank_row_and_column Eigentum

Gibt an, ob führende leere Zeilen und Spalten gekürzt werden sollen, wie es MS Excel tut.
Standard ist wahr.

###  Bemerkungen

Dasselbe gilt für die Regel in MS Excel, eine Zeile/Spalte wird nicht als leer angesehen, wenn sie einen benutzerdefinierten Stil hat.
auch wenn es keine Zelldaten enthält.
Beim Speichern im LightCells-Modus hat diese Option keine Auswirkung.
Der Benutzer sollte den Ausgangsbereich durch die Implementierung von [TxtSaveOptions.light_cells_data_provider](/cells/de/python-net/aspose.cells/txtsaveoptions#light_cells_data_provider) steuern
oder unter Angabe von [TxtSaveOptions.export_area](/cells/de/python-net/aspose.cells/txtsaveoptions#export_area)
###  Definition:
```python
@property
def trim_leading_blank_row_and_column(self):
    ...
@trim_leading_blank_row_and_column.setter
def trim_leading_blank_row_and_column(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [TxtSaveOptions](/cells/de/python-net/aspose.cells/txtsaveoptions)
