---
title: CellArea Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 150
url: /de/python-net/aspose.cells/cellarea/
is_root: false
---
##  CellArea Klasse
Stellen Sie einen Bereich von Zellen dar.



Der Typ CellArea macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [CellArea()](/cells/de/python-net/aspose.cells/cellarea/__init__/#) | Erstellt eine neue Instanz von CellArea|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [start_row](/cells/de/python-net/aspose.cells/cellarea/start_row) | Ruft die Startzeile dieses Bereichs ab oder legt sie fest.|
| [end_row](/cells/de/python-net/aspose.cells/cellarea/end_row) | Ruft die Endzeile dieses Bereichs ab oder legt sie fest.|
| [start_column](/cells/de/python-net/aspose.cells/cellarea/start_column) |Ruft die Startspalte dieses Bereichs ab oder legt sie fest.|
| [end_column](/cells/de/python-net/aspose.cells/cellarea/end_column) | Ruft die Endspalte dieses Bereichs ab oder legt sie fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [create_cell_area(start_row, start_column, end_row, end_column)](/cells/de/python-net/aspose.cells/cellarea/create_cell_area/#int-int-int-int) | Erstellt einen Zellbereich.|
| [create_cell_area(start_cell_name, end_cell_name)](/cells/de/python-net/aspose.cells/cellarea/create_cell_area/#str-str) | Erstellt einen Zellbereich.|
| [compare_to(obj)](/cells/de/python-net/aspose.cells/cellarea/compare_to/#any) | Vergleichen Sie zwei CellArea-Objekte entsprechend ihrer oberen linken Ecke.|



###  Beispiel

```python
from aspose.cells import CellArea

# Create Cell Area
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0

```

###  Siehe auch
* Modul [aspose.cells](..)
