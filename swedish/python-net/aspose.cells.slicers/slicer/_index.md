---
title: Slicer klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 10
url: /sv/python-net/aspose.cells.slicers/slicer/
is_root: false
---
##  Slicer klass
sammanfattande beskrivning av Slicer View



Typen Slicer avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [title](/cells/sv/python-net/aspose.cells.slicers/slicer/title) | Anger titeln på det aktuella Slicer-objektet.|
| [alternative_text](/cells/sv/python-net/aspose.cells.slicers/slicer/alternative_text) | Returnerar eller ställer in den beskrivande (alternativa) textsträngen för Slicer-objektet.|
| [is_printable](/cells/sv/python-net/aspose.cells.slicers/slicer/is_printable) | Indikerar om skivobjektet är utskrivbart.|
| [is_locked](/cells/sv/python-net/aspose.cells.slicers/slicer/is_locked) | Indikerar om skärformen är låst.|
| [placement](/cells/sv/python-net/aspose.cells.slicers/slicer/placement) | Representerar hur ritobjektet är fäst vid cellerna under det.<br/> Egenskapen styr placeringen av ett objekt på ett kalkylblad.|
| [locked_aspect_ratio](/cells/sv/python-net/aspose.cells.slicers/slicer/locked_aspect_ratio) | Indikerar om låsning av bildförhållande.|
| [locked_position](/cells/sv/python-net/aspose.cells.slicers/slicer/locked_position) | Indikerar om den angivna skivaren kan flyttas eller storleksändras med hjälp av användargränssnittet.|
| [slicer_cache](/cells/sv/python-net/aspose.cells.slicers/slicer/slicer_cache) | Returnerar SlicerCache-objektet som är associerat med slicern. Skrivskyddad.|
| [parent](/cells/sv/python-net/aspose.cells.slicers/slicer/parent) | Returnerar kalkylbladsobjektet som representerar arket som innehåller utsnittet. Skrivskyddad.|
| [style_type](/cells/sv/python-net/aspose.cells.slicers/slicer/style_type) | Ange typen av inbyggd slicerstil<br/> standardtypen är SlicerStyleLight1|
| [name](/cells/sv/python-net/aspose.cells.slicers/slicer/name) | Returnerar eller ställer in namnet på den angivna skivaren|
| [caption](/cells/sv/python-net/aspose.cells.slicers/slicer/caption) | Returnerar eller ställer in bildtexten för det angivna utsnittet.|
| [caption_visible](/cells/sv/python-net/aspose.cells.slicers/slicer/caption_visible) | Returnerar eller ställer in om rubriken som visar slicer Caption är synlig<br/> standardvärdet är sant|
| [number_of_columns](/cells/sv/python-net/aspose.cells.slicers/slicer/number_of_columns) |Returnerar eller ställer in antalet kolumner i det angivna utsnittet.|
| [left_pixel](/cells/sv/python-net/aspose.cells.slicers/slicer/left_pixel) | Returnerar eller ställer in den horisontella förskjutningen av utsnittsformen från dess vänstra kolumn, i pixlar.|
| [top_pixel](/cells/sv/python-net/aspose.cells.slicers/slicer/top_pixel) | Returnerar eller ställer in den vertikala förskjutningen av skivformen från dess översta raden, i pixlar.|
| [width](/cells/sv/python-net/aspose.cells.slicers/slicer/width) | Returnerar eller ställer in bredden på den angivna skivaren, i punkter.|
| [width_pixel](/cells/sv/python-net/aspose.cells.slicers/slicer/width_pixel) | Returnerar eller ställer in bredden på det angivna utsnittet, i pixlar.|
| [height](/cells/sv/python-net/aspose.cells.slicers/slicer/height) | Returnerar eller ställer in höjden på den angivna skivaren, i punkter.|
| [height_pixel](/cells/sv/python-net/aspose.cells.slicers/slicer/height_pixel) | Returnerar eller ställer in höjden på det angivna utsnittet i pixlar.|
| [column_width_pixel](/cells/sv/python-net/aspose.cells.slicers/slicer/column_width_pixel) | Hämtar eller ställer in bredden i pixelenhet för varje kolumn i utsnittet.|
| [column_width](/cells/sv/python-net/aspose.cells.slicers/slicer/column_width) | Returnerar eller ställer in bredden, i punkter, för varje kolumn i utsnittet.|
| [row_height_pixel](/cells/sv/python-net/aspose.cells.slicers/slicer/row_height_pixel) | Returnerar eller ställer in höjden, i pixlar, för varje rad i det angivna utsnittet.|
| [row_height](/cells/sv/python-net/aspose.cells.slicers/slicer/row_height) | Returnerar eller ställer in höjden, i punkter, för varje rad i den angivna slicern.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add_pivot_connection(pivot)](/cells/sv/python-net/aspose.cells.slicers/slicer/add_pivot_connection/#aspose.cells.pivot.PivotTable) | Lägger till PivotTable-anslutning.|
| [remove_pivot_connection(pivot)](/cells/sv/python-net/aspose.cells.slicers/slicer/remove_pivot_connection/#aspose.cells.pivot.PivotTable) | Tar bort PivotTable-anslutning.|
| [refresh()](/cells/sv/python-net/aspose.cells.slicers/slicer/refresh/#) | Uppdatera skivaren. Under tiden uppdaterar och beräknar relativa pivottabeller.|



###  Exempel

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
from aspose.cells.slicers import SlicerStyleType

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
pivot.refresh_data()
pivot.calculate_data()
slicers = sheet.slicers
slicerIndex = slicers.add(pivot, "E12", "fruit")
slicer = slicers[slicerIndex]
slicer.style_type = SlicerStyleType.SLICER_STYLE_LIGHT2
items = slicer.slicer_cache.slicer_cache_items
item = items[0]
item.selected = False
# do your business
book.save("out.xlsx")

```

###  Se även
* modul [aspose.cells.slicers](..)
