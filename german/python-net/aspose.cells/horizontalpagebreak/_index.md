---
title: HorizontalPageBreak Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 750
url: /de/python-net/aspose.cells/horizontalpagebreak/
is_root: false
---
##  HorizontalPageBreak Klasse
Kapselt das Objekt, das einen horizontalen Seitenumbruch darstellt.



Der Typ HorizontalPageBreak macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [start_column](/cells/de/python-net/aspose.cells/horizontalpagebreak/start_column) | Ruft den Startspaltenindex dieses horizontalen Seitenumbruchs ab.|
| [end_column](/cells/de/python-net/aspose.cells/horizontalpagebreak/end_column) |Ruft den Endspaltenindex dieses horizontalen Seitenumbruchs ab.|
| [row](/cells/de/python-net/aspose.cells/horizontalpagebreak/row) | Ruft den nullbasierten Zeilenindex ab.|



###  Beispiel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Add a page break at cell Y30
Index = worksheet.horizontal_page_breaks.add("Y30")
# get the newly added horizontal page break
hPageBreak = worksheet.horizontal_page_breaks[Index]

```

###  Siehe auch
* Modul [aspose.cells](..)
