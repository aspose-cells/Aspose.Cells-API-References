---
title: CommentCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 290
url: /sv/python-net/aspose.cells/commentcollection/
is_root: false
---
##  CommentCollection klass
Kapslar in en samling av [Comment](/cells/sv/python-net/aspose.cells/comment) objekt.



Typen CommentCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [capacity](/cells/sv/python-net/aspose.cells/commentcollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add_threaded_comment(row, column, text, author)](/cells/sv/python-net/aspose.cells/commentcollection/add_threaded_comment/#int-int-str-ThreadedCommentAuthor) | Lägger till en trådad kommentar.|
| [add_threaded_comment(cell_name, text, author)](/cells/sv/python-net/aspose.cells/commentcollection/add_threaded_comment/#str-str-ThreadedCommentAuthor) | Lägger till en trådad kommentar.|
| [get_threaded_comments(row, column)](/cells/sv/python-net/aspose.cells/commentcollection/get_threaded_comments/#int-int) | Får de trådade kommentarerna efter rad- och kolumnindex.|
| [get_threaded_comments(cell_name)](/cells/sv/python-net/aspose.cells/commentcollection/get_threaded_comments/#str) | Får de trådade kommentarerna efter cellnamn.|
| [add(row, column)](/cells/sv/python-net/aspose.cells/commentcollection/add/#int-int) | Lägger till en kommentar till samlingen.|
| [add(cell_name)](/cells/sv/python-net/aspose.cells/commentcollection/add/#str) | Lägger till en kommentar till samlingen.|
| [remove_at(cell_name)](/cells/sv/python-net/aspose.cells/commentcollection/remove_at/#str) | Tar bort kommentaren från den specifika cellen.|
| [remove_at(row, column)](/cells/sv/python-net/aspose.cells/commentcollection/remove_at/#int-int) | Tar bort kommentaren från den specifika cellen.|
| [copy_to(array)](/cells/sv/python-net/aspose.cells/commentcollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells/commentcollection/copy_to/#int-list-int-int) |Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells/commentcollection/index_of/#Comment-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells/commentcollection/index_of/#Comment-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells/commentcollection/last_index_of/#Comment) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells/commentcollection/binary_search/#Comment) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



###  Exempel

```python
from aspose.cells import Workbook

workbook = Workbook()
comments = workbook.worksheets[0].comments

```

###  Se även
* modul [aspose.cells](..)
* klass [Comment](/cells/sv/python-net/aspose.cells/comment)
