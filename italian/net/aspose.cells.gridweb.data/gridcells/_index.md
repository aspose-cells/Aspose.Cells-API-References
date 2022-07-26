---
title: GridCells
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula una raccolta diCell oggetti.
type: docs
weight: 190
url: /it/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

Incapsula una raccolta diCell oggetti.

```csharp
public class GridCells : IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.gridweb.data/gridcells/count) { get; } | Ottiene il numero di celle. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.gridweb.data/gridcells/item) { get; } | OttieneCell elemento all'interno del foglio di lavoro (3 indexers) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn) { get; } | Indice di colonna massimo della cella che contiene dati o stile. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow) { get; } | Indice di riga massimo della cella che contiene dati o stile. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells) { get; } | Ottiene la raccolta di celle unite. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator) { get; } | Ottiene l'enumeratore di righe |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows) { get; } |  |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight) { get; set; } | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di punti. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels) { get; set; } | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di pixel. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth) { get; set; } | Ottiene o imposta la larghezza della colonna predefinita nel foglio di lavoro, in unità di caratteri. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear)() | Cancella tutte le celle nella raccolta. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents#clearcontents)(GridCellArea) | Cancella il contenuto di un intervallo. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents#clearcontents_1)(int, int, int, int) | Cancella il contenuto di un intervallo. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats#clearformats)(GridCellArea) | Cancella la formattazione di un intervallo. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats#clearformats_1)(int, int, int, int) | Cancella la formattazione di un intervallo. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange#clearrange)(GridCellArea) | Cancella il contenuto e la formattazione di un intervallo. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange#clearrange_1)(int, int, int, int) | Cancella il contenuto e la formattazione di un intervallo. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn)(GridCells, int, int) | Copia i dati e le formattazioni di un'intera colonna. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns)(GridCells, int, int, int) | Copia i dati e le formattazioni di un'intera colonna. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow)(GridCells, int, int) | Copia i dati e le formattazioni di un'intera riga. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows)(GridCells, int, int, int) | Copia i dati e le formattazioni di alcune righe intere. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns)() | Elimina tutte le colonne vuote che non contengono dati. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows)() | Elimina tutte le righe vuote che non contengono dati. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn#deletecolumn)(int) | Elimina una colonna. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn#deletecolumn_1)(int, bool) | Elimina una colonna. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns)(int, int, bool) | Elimina diverse colonne. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange)(int, int, int, int, GridShiftType) | Elimina un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow)(int) | Elimina una riga. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows#deleterows)(int, int) | Elimina diverse righe. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows#deleterows_1)(int, int, bool) | Elimina più righe nel foglio di lavoro. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export)(int, int, int, int, bool, bool) | Esporta i dati nella raccolta Cells di un foglio di lavoro Web in un nuovo oggetto DataTable |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray)(int, int, int, int) | Esporta i dati nel fileCellsraccolta in un oggetto array a due dimensioni. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell)(int, int) | Ottiene ilCell elemento o null in corrispondenza dell'indice di riga della cella e dell'indice di colonna specificati. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth)(int) | Ottiene la larghezza della colonna specificata |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch)(int) | Ottiene la larghezza della colonna specificata, in unità di pollici. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel)(int) | Ottiene la larghezza della colonna specificata, in unità di pixel. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator)() | Ottiene l'enumeratore di righe |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow)(int) | Ottiene ilRow elemento o all'indice della riga della cella specificato. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight)(int) | Ottiene l'altezza di una riga specificata. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch)(int) | Ottiene l'altezza di una riga specificata in unità di pollici. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel)(int) | Ottiene l'altezza di una riga specificata in unità di pixel. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel)(int) | Ottiene il livello di struttura della riga. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel)(int) | Ottieni la larghezza in un diverso tipo di vista. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns#groupcolumns)(int, int) | Colonne dei gruppi. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns#groupcolumns_1)(int, int, bool) | Colonne dei gruppi. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows)(int, int) | Raggruppa righe. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn)(int) | Nasconde una colonna. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow)(int) | Nasconde una riga. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn#insertcolumn)(int) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn#insertcolumn_1)(int, bool) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns#insertcolumns)(int, int) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns#insertcolumns_1)(int, int, bool) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange#insertrange)(GridCellArea, GridShiftType) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange#insertrange_1)(GridCellArea, int, GridShiftType, bool) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow)(int) | Inserisce una nuova riga nel foglio di lavoro. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows#insertrows)(int, int) | Inserisce più righe nel foglio di lavoro. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows#insertrows_1)(int, int, bool) | Inserisce più righe nel foglio di lavoro. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn)(int) | Verifica se la colonna data è vuota (non contiene dati). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden)(int) | Verifica se una colonna in un determinato indice è nascosta. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden)(int) | Verifica se una riga in un determinato indice è nascosta. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge)(int, int, int, int) | Unisce un intervallo di celle specificato in una singola cella. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange)(GridCellArea, int, int) | Sposta l'intervallo. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas)() | Rimuove tutta la formula e la sostituisce con il valore della formula. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Imposta i bordi per un intervallo di celle. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth)(int, double) | Imposta la larghezza della colonna specificata. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch)(int, double) | Imposta la larghezza della colonna in unità di pollici. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel)(int, int) | Imposta la larghezza della colonna in unità di pixel. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight)(int, double) | Imposta l'altezza della riga specificata. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch)(int, double) | Imposta l'altezza della riga in unità di pollici. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel)(int, int) | Imposta l'altezza della riga in unità di pixel. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel)(int, int) | Imposta il livello di struttura della riga. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle#setstyle_1)(string, GridTableItemStyle) | Imposta lo stile su un intervallo di celle specificato. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle#setstyle)(int, int, int, int, GridTableItemStyle) | Imposta lo stile su un intervallo di celle specificato. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort#sort)(int, int, int, int, int, bool, bool, bool) | Ordina i dati ascendente/decrescente dall'alto verso il basso in un intervallo di un foglio di lavoro in base all'indice di colonna specificato. Ordina i dati ascendente/decrescente da sinistra a destra in un intervallo di un foglio di lavoro in base all'indice di riga specificato. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns)(int, int) | Separa le colonne. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows)(int, int) | Separa le righe. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn)(int, double) | Mostra una colonna |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow)(int) | Mostra una riga. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge)(int, int, int, int) | Separa un intervallo specificato di celle unite. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname)(int, int) | Ottiene il nome della cella in base ai relativi indici di riga e colonna. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex)(string, out int, out int) | Ottiene gli indici delle righe e delle colonne della cella in base al nome |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname)(int) | Ottiene il nome della colonna in base all'indice della colonna. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex)(string) | Ottiene l'indice della colonna in base al nome della colonna. |

### Guarda anche

* spazio dei nomi [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* assemblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
