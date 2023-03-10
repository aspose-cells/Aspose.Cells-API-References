---
title: update_linked_data_source metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 410
url: /sv/python-net/aspose.cells/workbook/update_linked_data_source/
is_root: false
---
##  update_linked_data_source(external_workbooks) {#list}
Om den här arbetsboken innehåller externa länkar till andra datakällor,
Aspose.Cells kommer att försöka hämta de senaste uppgifterna.



```python
def update_linked_data_source(self, external_workbooks):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| external_workbooks | list | Externa arbetsböcker refereras av denna arbetsbok.<br/>Om det är null öppnar vi de externt länkade filerna direkt.<br/> Om det inte är null,<br/>vi kommer att kontrollera om den externa länken i arrayen först;<br/> om inte kommer vi att öppna de externt länkade filerna igen.|
###  Anmärkningar

Om metoden inte anropas innan formler beräknas,
Aspose.Cells kommer att använda den tidigare informationen (cachelagrad i filen);
 Vänligen ställ in CellsHelper.StartupPath,CellsHelper.AltStartPath,CellsHelper.LibraryPath.
Och vänligen ställ in Workbook.FilePath om den här arbetsboken är från en ström,
annars kunde Aspose.Cells inte få den externa länkens fullständiga sökväg ibland.


###  Se även
* modul [aspose.cells](../../)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
