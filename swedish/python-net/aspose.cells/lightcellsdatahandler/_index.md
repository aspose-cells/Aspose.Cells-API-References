---
title: LightCellsDataHandler klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 990
url: /sv/python-net/aspose.cells/lightcellsdatahandler/
is_root: false
---
##  LightCellsDataHandler klass
Representerar celldatahanterare för att läsa stora kalkylbladsfiler i lättviktsläge.



Typen LightCellsDataHandler avslöjar följande medlemmar:

###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [start_sheet(sheet)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#Worksheet) | Börjar bearbeta ett kalkylblad.|
| [start_row(row_index)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) | Förbereder bearbetning av en rad.|
| [process_row(row)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/process_row/#Row) | Börjar bearbeta en rad.|
| [start_cell(column_index)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) | Förbereder att bearbeta en cell.|
| [process_cell(cell)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/process_cell/#Cell) | Börjar bearbeta en cell.|



###  Anmärkningar

När du läser en arbetsbok med det här läget, kommer [LightCellsDataHandler.start_sheet(sheet)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/start_sheet) att kontrolleras när du läser alla kalkylblad i arbetsboken.
För ett ark, om [LightCellsDataHandler.start_sheet(sheet)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/start_sheet) ger sant, kommer alla data och egenskaper för rader/celler i detta ark att kontrolleras
och bearbetas av implementeringen av detta gränssnitt. För varje rad kommer [LightCellsDataHandler.start_row(row_index)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/start_row) att anropas för att kontrollera om den behöver bearbetas.
Om en rad behöver bearbetas kommer egenskaperna för denna rad att läsas först och användaren kan komma åt dess egenskaper genom [LightCellsDataHandler.process_row(row)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/process_row).
om radens celler också behöver bearbetas, så ska [LightCellsDataHandler.process_row(row)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/process_row) returnera sant och då kommer [LightCellsDataHandler.start_cell(column_index)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/start_cell) att vara
uppmanade varje befintlig cell i den här raden att kontrollera om en cell behöver bearbetas. Om en cell behöver bearbetas,
då kommer [LightCellsDataHandler.process_cell(cell)](/cells/sv/python-net/aspose.cells/lightcellsdatahandler/process_cell) att anropas för att behandla cellen genom implementeringen av detta gränssnitt.

###  Se även
* modul [aspose.cells](..)
