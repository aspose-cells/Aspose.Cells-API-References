---
title: PictureCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 460
url: /sv/python-net/aspose.cells.drawing/picturecollection/
is_root: false
---
##  PictureCollection klass
Kapslar in en samling av [Picture](/cells/sv/python-net/aspose.cells.drawing/picture) objekt.



Typen PictureCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [capacity](/cells/sv/python-net/aspose.cells.drawing/picturecollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-io.RawIOBase) | Lägger till en bild i samlingen.|
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-str) | Lägger till en bild i samlingen.|
| [add(upper_left_row, upper_left_column, stream)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase) | Lägger till en bild i samlingen.|
| [add(upper_left_row, upper_left_column, file_name)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str) | Lägger till en bild i samlingen.|
| [add(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase-int-int) | Lägger till en bild i samlingen.|
| [add(upper_left_row, upper_left_column, file_name, width_scale, height_scale)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str-int-int) | Lägger till en bild i samlingen.|
| [copy_to(array)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/copy_to/#int-list-int-int) |Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells.drawing/picturecollection/binary_search/#Picture) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



###  Exempel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get PictureCollection
pictures = workbook.worksheets[0].pictures
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Se även
* modul [aspose.cells.drawing](..)
* klass [Picture](/cells/sv/python-net/aspose.cells.drawing/picture)
