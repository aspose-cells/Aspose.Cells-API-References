---
title: "Classe GridCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridDesktop.Data.GridCells class. Incapsula una raccolta di oggetti Cell"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Incapsula una raccolta di oggetti Cell.

```csharp
public class GridCells : IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns/) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count/) { get; } | Ottiene il numero di celle. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell/) { get; } | Ottiene la prima cella in questo foglio di lavoro. |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item/) { get; } | Ottiene l'elemento [`GridCell`](../gridcell/) all'indice di riga e colonna della cella specificati. (2 indicizzatori) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell/) { get; } | Ottiene l'ultima cella in questo foglio di lavoro. |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn/) { get; } | Indice massimo della colonna della cella che contiene dati o stile. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn/) { get; } | Indice di colonna massimo della cella che contiene dati. |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow/) { get; } | Indice di riga massimo della cella che contiene dati. |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow/) { get; } | Indice di riga massimo della cella che contiene dati o stile. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells/) { get; } | Ottiene la raccolta di celle unite. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn/) { get; } | Indice di colonna minimo delle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma non è stata istanziata alcuna cella). |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn/) { get; } | Indice di colonna minimo della cella che contiene dati. |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow/) { get; } | Indice di riga minimo della cella che contiene dati. |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow/) { get; } | Indice di riga minimo della cella che contiene dati o stile. |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator/) { get; } | Ottiene l'enumeratore delle righe |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows/) { get; } | Ottiene la raccolta di oggetti [`GridRow`](../gridrow/) che rappresentano le righe individuali in questo foglio di lavoro. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight/) { get; set; } | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels/) { get; set; } | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth/) { get; set; } | Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch/) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell/)(int, int) | Ottiene l'elemento [`GridCell`](../gridcell/) o null all'indice di riga e colonna della cella specificati. |
| [CheckRow](../../aspose.cells.griddesktop.data/gridcells/checkrow/)(int) | Ottiene l'elemento [`GridRow`](../gridrow/) o null all'indice di riga della cella specificato. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear/)() | Cancella tutte le celle nella raccolta. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Cancella il contenuto di un range. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Cancella il contenuto di un range. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats)(GridCellArea) | Cancella la formattazione di un range. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Cancella la formattazione di un range. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange)(GridCellArea) | Cancella il contenuto e la formattazione di un range. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Cancella il contenuto e la formattazione di un range. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn/)(GridCells, int, int) | Copia i dati e la formattazione di un'intera colonna. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns/)(GridCells, int, int, int) | Copia i dati e la formattazione di un'intera colonna. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow/)(GridCells, int, int) | Copia i dati e la formattazione di un'intera riga. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows/)(GridCells, int, int, int) | Copia i dati e la formattazione di alcune righe intere. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns/)() | Elimina tutte le colonne vuote che non contengono alcun dato. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows/)() | Elimina tutte le righe vuote che non contengono alcun dato. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn)(int) | Elimina una colonna. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Elimina una colonna. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns/)(int, int, bool) | Elimina diverse colonne. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow/)(int) | Elimina una riga. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows)(int, int) | Elimina diverse righe. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Elimina più righe nel foglio di lavoro. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle/)(int, int) | Ottieni lo stile della cella fornita. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn/)(int) | Ottiene l'elemento [`GridColumn`](../gridcolumn/) o all'indice di colonna della cella specificato. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth/)(int) | Ottiene la larghezza della colonna specificata |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch/)(int) | Ottiene la larghezza della colonna specificata, in unità di pollici. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel/)(int) | Ottiene la larghezza della colonna specificata, in unità di pixel. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator/)() | Ottiene l'enumeratore delle righe |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow/)(int) | Ottiene l'elemento [`GridRow`](../gridrow/) o all'indice di riga della cella specificato. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight/)(int) | Restituisce l'altezza di una riga specificata. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch/)(int) | Restituisce l'altezza di una riga specificata in unità di pollici. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel/)(int) | Restituisce l'altezza di una riga specificata in unità di pixel. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel/)(int) | Restituisce la larghezza in diversi tipi di visualizzazione. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Raggruppa le colonne. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Raggruppa le colonne. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows/)(int, int) | Raggruppa le righe. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn/)(int) | Nasconde una colonna. |
| [HideColumns](../../aspose.cells.griddesktop.data/gridcells/hidecolumns/)(int, int) | Nascondi più colonne. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow/)(int) | Nasconde una riga. |
| [HideRows](../../aspose.cells.griddesktop.data/gridcells/hiderows/)(int, int) | Nasconde più righe. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn)(int) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow/)(int) | Inserisce una nuova riga nel foglio di lavoro. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows)(int, int) | Inserisce più righe nel foglio di lavoro. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Inserisce più righe nel foglio di lavoro. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn/)(int) | Verifica se la colonna specificata è vuota (non contiene alcun dato). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden/)(int) | Verifica se una colonna all'indice specificato è nascosta. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden/)(int) | Verifica se una riga all'indice specificato è nascosta. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge/)(int, int, int, int) | Unisce un intervallo di celle specificato in un'unica cella. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas/)() | Rimuove tutte le formule e le sostituisce con il valore della formula. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth/)(int, double) | Imposta la larghezza della colonna specificata. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch/)(int, double) | Imposta la larghezza della colonna in unità di pollici. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel/)(int, int) | Imposta la larghezza della colonna in unità di pixel. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight/)(int, double) | Imposta l'altezza della riga specificata. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch/)(int, double) | Imposta l'altezza della riga in unità di pollici. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel/)(int, int) | Imposta l'altezza della riga in unità di pixel. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle)(CellRange, Style) | Imposta lo stile a un intervallo specificato di celle. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_2)(string, Style) | Imposta lo stile a un intervallo specificato di celle. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_1)(int, int, int, int, Style) | Imposta lo stile a un intervallo specificato di celle. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Ordina i dati in modo ascendente/decendente dall'alto verso il basso in un intervallo di un Worksheet secondo l'indice di colonna specificato. Ordina i dati in modo ascendente/decendente da sinistra a destra in un intervallo di un Worksheet secondo l'indice di riga specificato. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) | Ordina i dati dell'area. |
| [SortAsNumber](../../aspose.cells.griddesktop.data/gridcells/sortasnumber/)(int, int, int, int, int[], SortOrder[], SortOrientation) | Ordina i dati dell'area (i dati della colonna chiave devono essere numerici). |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns/)(int, int) | Separa le colonne dal raggruppamento. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows/)(int, int) | Separa le righe dal raggruppamento. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn/)(int, double) | Rende visibile una colonna |
| [UnhideColumns](../../aspose.cells.griddesktop.data/gridcells/unhidecolumns/)(int, int, double) | Rende visibili più colonne. |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow/)(int, int) | Rende visibile una riga. |
| [UnhideRows](../../aspose.cells.griddesktop.data/gridcells/unhiderows/)(int, int, double) | Rende visibili le righe nascoste. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge/)(int, int, int, int) | Separa un intervallo specificato di celle unite. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname/)(int, int) | Ottiene il nome della cella in base ai suoi indici di riga e colonna. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex/)(string, out int, out int) | Ottiene gli indici di riga e colonna della cella in base al suo nome |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname/)(int) | Ottiene il nome della colonna in base all'indice della colonna. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex/)(string) | Ottiene l'indice della colonna in base al nome della colonna. |

### Vedi anche

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


