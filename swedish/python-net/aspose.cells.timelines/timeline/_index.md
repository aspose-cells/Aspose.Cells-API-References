---
title: Timeline klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 10
url: /sv/python-net/aspose.cells.timelines/timeline/
is_root: false
---
##  Timeline klass
Sammanfattande beskrivning av Timeline Visa
På grund av MS Excel stöder inte Excel 2003 Timeline



Typen Timeline avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [caption](/cells/sv/python-net/aspose.cells.timelines/timeline/caption) | Returnerar eller ställer in bildtexten för den angivna tidslinjen.|
| [name](/cells/sv/python-net/aspose.cells.timelines/timeline/name) |Returnerar eller ställer in namnet på den angivna tidslinjen|
| [left_pixel](/cells/sv/python-net/aspose.cells.timelines/timeline/left_pixel) | Returnerar eller ställer in den horisontella förskjutningen av tidslinjeformen från dess vänstra kolumn, i pixlar.|
| [top_pixel](/cells/sv/python-net/aspose.cells.timelines/timeline/top_pixel) | Returnerar eller ställer in den vertikala förskjutningen av tidslinjeformen från dess översta rad, i pixlar.|
| [width_pixel](/cells/sv/python-net/aspose.cells.timelines/timeline/width_pixel) | Returnerar eller ställer in bredden på den angivna tidslinjen, i pixlar.|
| [height_pixel](/cells/sv/python-net/aspose.cells.timelines/timeline/height_pixel) | Returnerar eller ställer in höjden på den angivna tidslinjen, i pixlar.|



###  Exempel

```python
from aspose.cells import CellsFactory, Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
import datetime

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
# Create date style
dateStyle = CellsFactory().create_style()
dateStyle.custom = "m/d/yyyy"
cells.get(0, 1).value = "date"
cells.get(1, 1).value = datetime(2021, 2, 5)
cells.get(2, 1).value = datetime(2022, 3, 8)
cells.get(3, 1).value = datetime(2023, 4, 10)
cells.get(4, 1).value = datetime(2024, 5, 16)
# Set date style
cells.get(1, 1).set_style(dateStyle)
cells.get(2, 1).set_style(dateStyle)
cells.get(3, 1).set_style(dateStyle)
cells.get(4, 1).set_style(dateStyle)
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
pivots = sheet.pivot_tables
# Add a PivotTable
pivotIndex = pivots.add("=Sheet1!A1:C5", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "date")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Refresh PivotTable data
pivot.refresh_data()
pivot.calculate_data()
# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 10, 5, "date")
# Get Timeline object
timelineObj = sheet.timelines[0]
# do your business
book.save("out.xlsx")

```

###  Se även
* modul [aspose.cells.timelines](..)
