---
title: LightCellsDataProvider klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1000
url: /sv/python-net/aspose.cells/lightcellsdataprovider/
is_root: false
---
##  LightCellsDataProvider klass
Representerar dataleverantör för att spara stora kalkylbladsfiler i lättviktsläge.



Typen LightCellsDataProvider avslöjar följande medlemmar:

###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [start_sheet(sheet_index)](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) | Börjar spara ett kalkylblad.|
| [next_row()](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/next_row/#) | Hämtar nästa rad som ska sparas.|
| [start_row(row)](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/start_row/#Row) | Börjar spara data på en rad.|
| [next_cell()](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) | Hämtar nästa cell som ska sparas.|
| [start_cell(cell)](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/start_cell/#Cell) | Börjar spara data från en cell.|
| [is_gather_string()](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) |Kontrollerar om det aktuella strängvärdet för cellen måste samlas in i en global pool.|



###  Anmärkningar

När du sparar en arbetsbok med det här läget, kommer [LightCellsDataProvider.start_sheet(sheet_index)](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/start_sheet) att kontrolleras när du sparar varje kalkylblad i arbetsboken.
För ett ark, om [LightCellsDataProvider.start_sheet(sheet_index)](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/start_sheet) ger sant, så ska alla data och egenskaper för rader/celler i detta ark sparas
kommer att tillhandahållas av implementeringen av detta gränssnitt. I första hand kommer [LightCellsDataProvider.next_row()](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/next_row) att anropas för att få nästa radindex som ska sparas.
Om ett giltigt radindex returneras (radindexet måste vara i stigande ordning för att raderna ska sparas),
sedan kommer ett Row-objekt som representerar denna rad att tillhandahållas för implementering för att ställa in dess egenskaper med [LightCellsDataProvider.start_row(row)](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/start_row).
För en rad kommer [LightCellsDataProvider.next_cell()](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/next_cell) först att kontrolleras. Om ett giltigt kolumnindex returneras (kolumnindexet måste vara i stigande ordning för att alla celler i en rad ska sparas),
sedan kommer ett Cell-objekt som representerar denna cell att tillhandahållas för implementering för att ställa in dess data och egenskaper med [LightCellsDataProvider.start_cell(cell)](/cells/sv/python-net/aspose.cells/lightcellsdataprovider/start_cell).
Efter att data för denna cell har ställts in, kommer denna cell att sparas direkt i den genererade kalkylbladsfilen och nästa cell kommer att kontrolleras och bearbetas.

###  Se även
* modul [aspose.cells](..)
