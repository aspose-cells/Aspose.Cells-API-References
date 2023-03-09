---
title: subtotal metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 920
url: /sv/python-net/aspose.cells/cells/subtotal/
is_root: false
---
##  subtotal(ca, group_by, function, total_list) {#CellArea-int-ConsolidationFunction-list}
Skapar delsummor för intervallet.



```python
def subtotal(self, ca, group_by, function, total_list):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| ca | [CellArea](/cells/sv/python-net/aspose.cells/cellarea) | Räckvidden|
| group_by | int | Fältet att gruppera efter, som en nollbaserad heltalsoffset|
| function | [ConsolidationFunction](/cells/sv/python-net/aspose.cells/consolidationfunction) | Subtotalfunktionen.|
| total_list | list | En matris med nollbaserade fältförskjutningar, som indikerar de fält till vilka delsummorna läggs till.|


##  subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data) {#CellArea-int-ConsolidationFunction-list-bool-bool-bool}
Skapar delsummor för intervallet.



```python
def subtotal(self, ca, group_by, function, total_list, replace, page_breaks, summary_below_data):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| ca | [CellArea](/cells/sv/python-net/aspose.cells/cellarea) | Räckvidden|
| group_by | int | Fältet att gruppera efter, som en nollbaserad heltalsoffset|
| function | [ConsolidationFunction](/cells/sv/python-net/aspose.cells/consolidationfunction) | Subtotalfunktionen.|
| total_list | list | En matris med nollbaserade fältförskjutningar, som indikerar de fält till vilka delsummorna läggs till.|
| replace | bool |Anger om de nuvarande delsummorna ersätts|
| page_breaks | bool | Anger om man lägger till sidbrytning mellan grupper|
| summary_below_data | bool | Anger om du lägger till sammanfattning nedanför data.|



###  Se även
* modul [aspose.cells](../../)
* klass [Cells](/cells/sv/python-net/aspose.cells/cells)
