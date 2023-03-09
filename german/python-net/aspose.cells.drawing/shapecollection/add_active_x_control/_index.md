---
title: add_active_x_control Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/
is_root: false
---
##  add_active_x_control(type, top_row, top, left_column, left, width, height) {#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int}
Erstellt ein Activex-Steuerelement.


###  Kehrt zurück




```python
def add_active_x_control(self, type, top_row, top, left_column, left, width, height):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | aspose.cells.drawing.activexcontrols.ControlType | Der Typ des Steuerelements.|
| top_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Versatz von Shape von seiner linken Zeile in Pixeleinheiten dar.|
| left_column | int | Spaltenindex oben links.|
| left | int | Stellt den horizontalen Versatz von Shape von seiner linken Spalte in Pixeleinheiten dar.|
| width | int | Stellt die Breite von Shape in Pixeleinheiten dar.|
| height | int | Stellt die Höhe von Shape in Pixeleinheiten dar.|

###  Beispiele

```python
from aspose.cells.drawing.activexcontrols import ControlType

# add an ActiveX control
activeXControl = shapes.add_active_x_control(ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
