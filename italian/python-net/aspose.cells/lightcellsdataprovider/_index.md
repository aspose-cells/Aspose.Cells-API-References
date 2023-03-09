---
title: classe LightCellsDataProvider
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1000
url: /it/python-net/aspose.cells/lightcellsdataprovider/
is_root: false
---
##  classe LightCellsDataProvider
Rappresenta il fornitore di dati per il salvataggio di file di fogli di calcolo di grandi dimensioni in modalità leggera.



Il tipo LightCellsDataProvider espone i membri seguenti:

###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [start_sheet(sheet_index)](/cells/it/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) | Inizia a salvare un foglio di lavoro.|
| [next_row()](/cells/it/python-net/aspose.cells/lightcellsdataprovider/next_row/#) | Ottiene la riga successiva da salvare.|
| [start_row(row)](/cells/it/python-net/aspose.cells/lightcellsdataprovider/start_row/#Row) | Inizia a salvare i dati di una riga.|
| [next_cell()](/cells/it/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) | Ottiene la cella successiva da salvare.|
| [start_cell(cell)](/cells/it/python-net/aspose.cells/lightcellsdataprovider/start_cell/#Cell) | Inizia a salvare i dati di una cella.|
| [is_gather_string()](/cells/it/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) |Controlla se il valore di stringa corrente della cella deve essere raccolto in un pool globale.|



###  Osservazioni

Quando si salva una cartella di lavoro in questa modalità, [LightCellsDataProvider.start_sheet(sheet_index)](/cells/it/python-net/aspose.cells/lightcellsdataprovider/start_sheet) verrà controllato durante il salvataggio di ogni foglio di lavoro nella cartella di lavoro.
Per un foglio, se [LightCellsDataProvider.start_sheet(sheet_index)](/cells/it/python-net/aspose.cells/lightcellsdataprovider/start_sheet) restituisce true, tutti i dati e le proprietà delle righe/celle di questo foglio devono essere salvati
sarà fornito dall'implementazione di questa interfaccia. In primo luogo, verrà chiamato [LightCellsDataProvider.next_row()](/cells/it/python-net/aspose.cells/lightcellsdataprovider/next_row) per ottenere l'indice di riga successivo da salvare.
Se viene restituito un indice di riga valido (l'indice di riga deve essere in ordine crescente affinché le righe vengano salvate),
quindi verrà fornito un oggetto Row che rappresenta questa riga per l'implementazione per impostarne le proprietà entro [LightCellsDataProvider.start_row(row)](/cells/it/python-net/aspose.cells/lightcellsdataprovider/start_row).
Per una riga, [LightCellsDataProvider.next_cell()](/cells/it/python-net/aspose.cells/lightcellsdataprovider/next_cell) verrà controllato per primo. Se viene restituito un indice di colonna valido (l'indice di colonna deve essere in ordine crescente per salvare tutte le celle di una riga),
quindi verrà fornito un oggetto Cell che rappresenta questa cella per l'implementazione per impostarne i dati e le proprietà entro [LightCellsDataProvider.start_cell(cell)](/cells/it/python-net/aspose.cells/lightcellsdataprovider/start_cell).
Dopo aver impostato i dati di questa cella, questa cella verrà salvata direttamente nel file del foglio di calcolo generato e la cella successiva verrà controllata ed elaborata.

###  Guarda anche
* modulo [aspose.cells](..)
