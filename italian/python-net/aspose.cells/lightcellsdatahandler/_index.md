---
title: classe LightCellsDataHandler
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 990
url: /it/python-net/aspose.cells/lightcellsdatahandler/
is_root: false
---
##  classe LightCellsDataHandler
Rappresenta il gestore dati delle celle per la lettura di file di fogli di calcolo di grandi dimensioni in modalità leggera.



Il tipo LightCellsDataHandler espone i membri seguenti:

###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [start_sheet(sheet)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#Worksheet) | Avvia l'elaborazione di un foglio di lavoro.|
| [start_row(row_index)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) |Si prepara a elaborare una riga.|
| [process_row(row)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/process_row/#Row) | Inizia a elaborare una riga.|
| [start_cell(column_index)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) | Si prepara a processare una cella.|
| [process_cell(cell)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/process_cell/#Cell) | Inizia a elaborare una cella.|



###  Osservazioni

Quando si legge una cartella di lavoro in questa modalità, [LightCellsDataHandler.start_sheet(sheet)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/start_sheet) verrà controllato durante la lettura di ogni foglio di lavoro nella cartella di lavoro.
Per un foglio, se [LightCellsDataHandler.start_sheet(sheet)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/start_sheet) restituisce true, verranno controllati tutti i dati e le proprietà delle righe/celle di questo foglio
ed elaborati dall'implementazione di questa interfaccia. Per ogni riga verrà chiamato lo [LightCellsDataHandler.start_row(row_index)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/start_row) per verificare se è necessario elaborarlo.
Se una riga deve essere elaborata, le proprietà di questa riga verranno lette per prime e l'utente potrà accedere alle sue proprietà entro il numero [LightCellsDataHandler.process_row(row)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/process_row).
se anche le celle della riga devono essere elaborate, allora [LightCellsDataHandler.process_row(row)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/process_row) dovrebbe restituire true e quindi [LightCellsDataHandler.start_cell(column_index)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/start_cell) sarà
chiamato per ogni cella esistente in questa riga per verificare se una cella deve essere elaborata. Se una cella deve essere elaborata,
quindi [LightCellsDataHandler.process_cell(cell)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/process_cell) verrà chiamato per elaborare la cella mediante l'implementazione di questa interfaccia.

###  Guarda anche
* modulo [aspose.cells](..)
