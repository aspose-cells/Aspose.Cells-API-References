---
title: GridCells
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula una raccolta diCelloggetti.
type: docs
weight: 410
url: /it/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Incapsula una raccolta diCelloggetti.

```csharp
public class GridCells : IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count) { get; } | Ottiene il numero di celle. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item) { get; } | OttieneCell elemento all'interno del foglio di lavoro (3 indexers) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn) { get; } | Indice di colonna massimo della cella che contiene dati o stile. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow) { get; } | Indice di riga massimo della cella che contiene dati o stile. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells) { get; } | Ottiene la raccolta di celle unite. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator) { get; } | Ottiene l'enumeratore di righe |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows) { get; } | Ottiene la raccolta di[`GridRow`](../gridrow) oggetti che rappresentano le singole righe in questo foglio di lavoro. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight) { get; set; } | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di punti. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels) { get; set; } | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di pixel. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth) { get; set; } | Ottiene o imposta la larghezza della colonna predefinita nel foglio di lavoro, in unità di caratteri. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell)(int, int) | Ottiene ilCell elemento o null in corrispondenza dell'indice di riga della cella e dell'indice di colonna specificati. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear)() | Cancella tutte le celle nella raccolta. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents#clearcontents)(GridCellArea) | Cancella il contenuto di un intervallo. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents#clearcontents_1)(int, int, int, int) | Cancella il contenuto di un intervallo. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats#clearformats)(GridCellArea) | Cancella la formattazione di un intervallo. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats#clearformats_1)(int, int, int, int) | Cancella la formattazione di un intervallo. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange#clearrange)(GridCellArea) | Cancella il contenuto e la formattazione di un intervallo. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange#clearrange_1)(int, int, int, int) | Cancella il contenuto e la formattazione di un intervallo. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn)(GridCells, int, int) | Copia i dati e le formattazioni di un'intera colonna. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns)(GridCells, int, int, int) | Copia i dati e le formattazioni di un'intera colonna. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow)(GridCells, int, int) | Copia i dati e le formattazioni di un'intera riga. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows)(GridCells, int, int, int) | Copia i dati e le formattazioni di alcune righe intere. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns)() | Elimina tutte le colonne vuote che non contengono dati. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows)() | Elimina tutte le righe vuote che non contengono dati. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn#deletecolumn)(int) | Elimina una colonna. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn#deletecolumn_1)(int, bool) | Elimina una colonna. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns)(int, int, bool) | Elimina diverse colonne. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow)(int) | Elimina una riga. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows#deleterows)(int, int) | Elimina diverse righe. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows#deleterows_1)(int, int, bool) | Elimina più righe nel foglio di lavoro. |
| [GetCell](../../aspose.cells.griddesktop.data/gridcells/getcell)(int, int) | Ottiene ilCell elemento o null in corrispondenza dell'indice di riga della cella e dell'indice di colonna specificati. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle)(int, int) | Ottieni lo stile della cella data. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn)(int) | Ottiene il[`GridColumn`](../gridcolumn) elemento o all'indice della colonna della cella specificato. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth)(int) | Ottiene la larghezza della colonna specificata |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch)(int) | Ottiene la larghezza della colonna specificata, in unità di pollici. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel)(int) | Ottiene la larghezza della colonna specificata, in unità di pixel. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator)() | Ottiene l'enumeratore di righe |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow)(int) | Ottiene il[`GridRow`](../gridrow) elemento o all'indice della riga della cella specificato. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight)(int) | Ottiene l'altezza di una riga specificata. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch)(int) | Ottiene l'altezza di una riga specificata in unità di pollici. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel)(int) | Ottiene l'altezza di una riga specificata in unità di pixel. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel)(int) | Ottieni la larghezza in un diverso tipo di vista. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns#groupcolumns)(int, int) | Colonne dei gruppi. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns#groupcolumns_1)(int, int, bool) | Colonne dei gruppi. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows)(int, int) | Raggruppa righe. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn)(int) | Nasconde una colonna. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow)(int) | Nasconde una riga. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn#insertcolumn)(int) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn#insertcolumn_1)(int, bool) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns#insertcolumns)(int, int) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns#insertcolumns_1)(int, int, bool) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow)(int) | Inserisce una nuova riga nel foglio di lavoro. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows#insertrows)(int, int) | Inserisce più righe nel foglio di lavoro. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows#insertrows_1)(int, int, bool) | Inserisce più righe nel foglio di lavoro. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn)(int) | Verifica se la colonna data è vuota (non contiene dati). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden)(int) | Verifica se una colonna in un determinato indice è nascosta. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden)(int) | Verifica se una riga in un determinato indice è nascosta. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge)(int, int, int, int) | Unisce un intervallo di celle specificato in una singola cella. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas)() | Rimuove tutta la formula e la sostituisce con il valore della formula. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth)(int, double) | Imposta la larghezza della colonna specificata. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch)(int, double) | Imposta la larghezza della colonna in unità di pollici. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel)(int, int) | Imposta la larghezza della colonna in unità di pixel. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight)(int, double) | Imposta l'altezza della riga specificata. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch)(int, double) | Imposta l'altezza della riga in unità di pollici. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel)(int, int) | Imposta l'altezza della riga in unità di pixel. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle)(CellRange, Style) | Imposta lo stile su un intervallo di celle specificato. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle_2)(string, Style) | Imposta lo stile su un intervallo di celle specificato. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle_1)(int, int, int, int, Style) | Imposta lo stile su un intervallo di celle specificato. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort#sort)(int, int, int, int, int, bool, bool, bool) | Ordina i dati ascendente/decrescente dall'alto verso il basso in un intervallo di un foglio di lavoro in base all'indice di colonna specificato. Ordina i dati ascendente/decrescente da sinistra a destra in un intervallo di un foglio di lavoro in base all'indice di riga specificato. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns)(int, int) | Separa le colonne. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows)(int, int) | Separa le righe. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn)(int, double) | Mostra una colonna |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow)(int) | Mostra una riga. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge)(int, int, int, int) | Separa un intervallo specificato di celle unite. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname)(int, int) | Ottiene il nome della cella in base ai relativi indici di riga e colonna. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex)(string, out int, out int) | Ottiene gli indici delle righe e delle colonne della cella in base al nome |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname)(int) | Ottiene il nome della colonna in base all'indice della colonna. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex)(string) | Ottiene l'indice della colonna in base al nome della colonna. |

### Guarda anche

* spazio dei nomi [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* assemblea [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
