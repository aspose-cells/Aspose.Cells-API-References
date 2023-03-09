---
title: VerticalPageBreak Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1560
url: /de/python-net/aspose.cells/verticalpagebreak/
is_root: false
---
##  VerticalPageBreak Klasse
Kapselt das Objekt, das einen vertikalen Seitenumbruch darstellt.



Der Typ VerticalPageBreak macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [start_row](/cells/de/python-net/aspose.cells/verticalpagebreak/start_row) | Ruft den Startzeilenindex des vertikalen Seitenumbruchs ab.|
| [end_row](/cells/de/python-net/aspose.cells/verticalpagebreak/end_row) | Ruft den Endzeilenindex des vertikalen Seitenumbruchs ab.|
| [column](/cells/de/python-net/aspose.cells/verticalpagebreak/column) | Ruft den Spaltenindex des vertikalen Seitenumbruchs ab.|



###  Beispiele

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Siehe auch
* Modul [aspose.cells](..)
