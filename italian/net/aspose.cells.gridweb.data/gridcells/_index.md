---
title: "Classe GridCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridCells. Incapsula una raccolta di oggetti GridCell"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

Incapsula una raccolta di oggetti [`GridCell`](../gridcell/).

```csharp
public class GridCells : IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns/) { get; } | Ottiene la raccolta di oggetti [`GridColumn`](../gridcolumn/) che rappresentano le colonne individuali in questo foglio di lavoro. |
| [Count](../../aspose.cells.gridweb.data/gridcells/count/) { get; } | Ottiene il numero di celle. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell/) { get; } | Ottiene la prima cella in questo foglio di lavoro. |
| [Item](../../aspose.cells.gridweb.data/gridcells/item/) { get; } | Ottiene l'elemento [`GridCell`](../gridcell/) all'indice di riga e colonna della cella specificati. (2 indicizzatori) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell/) { get; } | Ottiene l'ultima cella in questo foglio di lavoro. |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn/) { get; } | Indice massimo della colonna della cella che contiene dati o stile. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn/) { get; } | Indice di colonna massimo della cella che contiene dati. |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow/) { get; } | Indice di riga massimo della cella che contiene dati. |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow/) { get; } | Indice di riga massimo della cella che contiene dati o stile. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells/) { get; } | Ottiene la raccolta di celle unite. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn/) { get; } | Indice di colonna minimo delle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma non è stata istanziata alcuna cella). |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn/) { get; } | Indice di colonna minimo della cella che contiene dati. |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow/) { get; } | Indice di riga minimo della cella che contiene dati. |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow/) { get; } | Indice di riga minimo della cella che contiene dati o stile. |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator/) { get; } | Ottiene l'enumeratore delle righe |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows/) { get; } | Ottiene la raccolta di oggetti [`GridRow`](../gridrow/) che rappresentano le righe individuali in questo foglio di lavoro. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight/) { get; set; } | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels/) { get; set; } | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth/) { get; set; } | Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch/) { get; set; } | Ottiene o imposta la larghezza di colonna predefinita nel foglio di lavoro, in unità di pollici. |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels/) { get; set; } | Ottiene o imposta la larghezza di colonna predefinita nel foglio di lavoro, in unità di pixel. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CheckCell](../../aspose.cells.gridweb.data/gridcells/checkcell/)(int, int) | Ottiene l'elemento [`GridCell`](../gridcell/) o null all'indice di riga e colonna della cella specificati. |
| [CheckColumn](../../aspose.cells.gridweb.data/gridcells/checkcolumn/)(int) | Ottiene l'elemento [`GridColumn`](../gridcolumn/) o null all'indice di colonna specificato. |
| [CheckRow](../../aspose.cells.gridweb.data/gridcells/checkrow/)(int) | Ottiene l'elemento [`GridRow`](../gridrow/) o null all'indice di riga della cella specificato. |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear/)() | Cancella tutte le celle nella raccolta. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Cancella il contenuto di un range. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Cancella il contenuto di un range. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats)(GridCellArea) | Cancella la formattazione di un range. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Cancella la formattazione di un range. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange)(GridCellArea) | Cancella il contenuto e la formattazione di un range. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Cancella il contenuto e la formattazione di un range. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn/)(GridCells, int, int) | Copia i dati e la formattazione di un'intera colonna. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns/)(GridCells, int, int, int) | Copia i dati e la formattazione di un'intera colonna. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow/)(GridCells, int, int) | Copia i dati e la formattazione di un'intera riga. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows/)(GridCells, int, int, int) | Copia i dati e la formattazione di alcune righe intere. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns/)() | Elimina tutte le colonne vuote che non contengono alcun dato. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows/)() | Elimina tutte le righe vuote che non contengono alcun dato. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn)(int) | Elimina una colonna. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Elimina una colonna. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns/)(int, int, bool) | Elimina diverse colonne. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange/)(int, int, int, int, GridShiftType) | Elimina un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow/)(int) | Elimina una riga. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows)(int, int) | Elimina diverse righe. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Elimina più righe nel foglio di lavoro. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export/)(int, int, int, int, bool, bool) | Esporta i dati nella raccolta Cells di un WebWorksheet in un nuovo oggetto DataTable |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray/)(int, int, int, int) | Esporta i dati nella raccolta `GridCells` in un oggetto array bidimensionale. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell/)(int, int) | Ottiene l'elemento [`GridCell`](../gridcell/) all'indice di riga e colonna della cella specificati. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth/)(int) | Ottiene la larghezza della colonna specificata |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch/)(int) | Ottiene la larghezza della colonna specificata, in unità di pollici. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel/)(int) | Ottiene la larghezza della colonna specificata, in unità di pixel. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator/)() | Ottiene l'enumeratore delle righe |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow/)(int) | Ottiene l'elemento [`GridRow`](../gridrow/) o all'indice di riga della cella specificato. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight/)(int) | Restituisce l'altezza di una riga specificata. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch/)(int) | Restituisce l'altezza di una riga specificata in unità di pollici. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel/)(int) | Restituisce l'altezza di una riga specificata in unità di pixel. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel/)(int) | Ottiene il livello di contorno della riga. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel/)(int) | Restituisce la larghezza in diversi tipi di visualizzazione. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Raggruppa le colonne. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Raggruppa le colonne. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows/)(int, int) | Raggruppa le righe. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn/)(int) | Nasconde una colonna. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow/)(int) | Nasconde una riga. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn)(int) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange)(GridCellArea, GridShiftType) | Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange_1)(GridCellArea, int, GridShiftType, bool) | Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow/)(int) | Inserisce una nuova riga nel foglio di lavoro. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows)(int, int) | Inserisce più righe nel foglio di lavoro. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Inserisce più righe nel foglio di lavoro. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn/)(int) | Verifica se la colonna specificata è vuota (non contiene alcun dato). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden/)(int) | Verifica se una colonna all'indice specificato è nascosta. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden/)(int) | Verifica se una riga all'indice specificato è nascosta. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge/)(int, int, int, int) | Unisce un intervallo di celle specificato in un'unica cella. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange/)(GridCellArea, int, int) | Sposta l'intervallo. |
| [RemoveDuplicates](../../aspose.cells.gridweb.data/gridcells/removeduplicates/)(int, int, int, int) | Rimuove i valori duplicati nell'intervallo. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas/)() | Rimuove tutte le formule e le sostituisce con il valore della formula. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Imposta i bordi per un intervallo di celle. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth/)(int, double) | Imposta la larghezza della colonna specificata. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch/)(int, double) | Imposta la larghezza della colonna in unità di pollici. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel/)(int, int) | Imposta la larghezza della colonna in unità di pixel. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight/)(int, double) | Imposta l'altezza della riga specificata. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch/)(int, double) | Imposta l'altezza della riga in unità di pollici. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel/)(int, int) | Imposta l'altezza della riga in unità di pixel. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel/)(int, int) | Imposta il livello di contorno della riga. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle_1)(string, GridTableItemStyle) | Imposta lo stile a un intervallo specificato di celle. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle)(int, int, int, int, GridTableItemStyle) | Imposta lo stile a un intervallo specificato di celle. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Ordina i dati in modo ascendente/decendente dall'alto verso il basso in un intervallo di un Worksheet secondo l'indice di colonna specificato. Ordina i dati in modo ascendente/decendente da sinistra a destra in un intervallo di un Worksheet secondo l'indice di riga specificato. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Ordina i dati in modo ascendente/decendente dall'alto verso il basso in un intervallo di un Worksheet secondo l'indice di colonna specificato. Ordina i dati in modo ascendente/decendente da sinistra a destra in un intervallo di un Worksheet secondo l'indice di riga specificato. |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns/)(int, int) | Separa le colonne dal raggruppamento. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows/)(int, int) | Separa le righe dal raggruppamento. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn/)(int, double) | Rende visibile una colonna |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow/)(int) | Rende visibile una riga. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge/)(int, int, int, int) | Separa un intervallo specificato di celle unite. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname/)(int, int) | Ottiene il nome della cella in base ai suoi indici di riga e colonna. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex/)(string, out int, out int) | Ottiene gli indici di riga e colonna della cella in base al suo nome |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname/)(int) | Ottiene il nome della colonna in base all'indice della colonna. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex/)(string) | Ottiene l'indice della colonna in base al nome della colonna. |

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


