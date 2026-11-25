---
title: "Classe Cells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Cells. Incapsula una raccolta di oggetti pertinenti alle celle come Cell Row ...etc"
type: docs
url: /it/net/aspose.cells/cells/
---
## Cells class

Incapsula una raccolta di oggetti pertinenti alle celle, come [`Cell`](../cell/), [`Row`](../row/), ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns/) { get; } | Ottiene la raccolta di oggetti [`Column`](../column/) che rappresentano le singole colonne in questo foglio di lavoro. |
| [Count](../../aspose.cells/cells/count/) { get; } | Ottiene il conteggio totale degli oggetti Cell istanziati. |
| [CountLarge](../../aspose.cells/cells/countlarge/) { get; } | Ottiene il conteggio totale degli oggetti Cell istanziati. |
| [FirstCell](../../aspose.cells/cells/firstcell/) { get; } | Ottiene la prima cella in questo foglio di lavoro. |
| [IsDefaultColumnHidden](../../aspose.cells/cells/isdefaultcolumnhidden/) { get; set; } |  |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched/) { get; set; } | Indica che l'altezza della riga e l'altezza predefinita del carattere corrispondono |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden/) { get; set; } | Indica se la riga è nascosta per impostazione predefinita. |
| [Item](../../aspose.cells/cells/item/) { get; } | Ottiene l'elemento [`Cell`](../cell/) all'indice di riga e colonna della cella specificati. (2 indicizzatori) |
| [LastCell](../../aspose.cells/cells/lastcell/) { get; } | Ottiene l'ultima cella in questo foglio di lavoro. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn/) { get; } | Indice di colonna massimo delle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma non è stata istanziata alcuna cella). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn/) { get; } | Indice di colonna massimo della cella che contiene dati. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow/) { get; } | Indice di riga massimo della cella che contiene dati. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange/) { get; } | Ottiene l'intervallo massimo che include dati, celle unite e forme. |
| [MaxRow](../../aspose.cells/cells/maxrow/) { get; } | Indice di riga massimo della cella che contiene dati o stile. |
| [MemorySetting](../../aspose.cells/cells/memorysetting/) { get; set; } | Ottiene o imposta l'opzione di utilizzo della memoria per queste celle. |
| [MergedCells](../../aspose.cells/cells/mergedcells/) { get; } | (**Obsoleto.**) Ottiene la raccolta di celle unite. |
| [MinColumn](../../aspose.cells/cells/mincolumn/) { get; } | Indice di colonna minimo delle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma non è stata istanziata alcuna cella). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn/) { get; } | Indice di colonna minimo della cella che contiene dati. |
| [MinDataRow](../../aspose.cells/cells/mindatarow/) { get; } | Indice di riga minimo della cella che contiene dati. |
| [MinRow](../../aspose.cells/cells/minrow/) { get; } | Indice di riga minimo della cella che contiene dati o stile. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading/) { get; set; } | Ottiene o imposta se il modello dati delle celle deve supportare la lettura Multi-Thread. Il valore predefinito di questa proprietà è false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields/) { get; } | Ottiene l'elenco dei campi di ods. |
| [PreserveString](../../aspose.cells/cells/preservestring/) { get; set; } | Ottiene o imposta un valore che indica se tutti i valori del foglio di lavoro sono conservati come stringhe. Il valore predefinito è false. |
| [Ranges](../../aspose.cells/cells/ranges/) { get; } | Ottiene la raccolta di oggetti [`Range`](../range/) creati a runtime. |
| [Rows](../../aspose.cells/cells/rows/) { get; } | Ottiene la raccolta di oggetti [`Row`](../row/) che rappresentano le singole righe in questo foglio di lavoro. |
| [StandardHeight](../../aspose.cells/cells/standardheight/) { get; set; } | Ottiene o imposta l'altezza di riga predefinita in questo foglio di lavoro, in unità di punti. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch/) { get; set; } | Ottiene o imposta l'altezza di riga predefinita in questo foglio di lavoro, in unità di pollici. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels/) { get; set; } | Ottiene o imposta l'altezza di riga predefinita in questo foglio di lavoro, in unità di pixel. |
| [StandardWidth](../../aspose.cells/cells/standardwidth/) { get; set; } | Ottiene o imposta la larghezza di colonna predefinita nel foglio di lavoro, in unità di caratteri. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch/) { get; set; } | Ottiene o imposta la larghezza di colonna predefinita nel foglio di lavoro, in unità di pollici. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels/) { get; set; } | Ottiene o imposta la larghezza di colonna predefinita nel foglio di lavoro, in unità di pixel. |
| [Style](../../aspose.cells/cells/style/) { get; set; } | Ottiene e imposta lo stile predefinito del foglio di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange/)(Range) | Aggiunge un riferimento a un oggetto range alle celle. |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle/)(int, Style, StyleFlag) | Applica formati a un'intera colonna. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle/)(int, Style, StyleFlag) | Applica formati a un'intera riga. |
| [ApplyStyle](../../aspose.cells/cells/applystyle/)(Style, StyleFlag) | Applica formati a un intero foglio di lavoro. |
| [CheckCell](../../aspose.cells/cells/checkcell/)(int, int) | Ottiene l'elemento [`Cell`](../cell/) o null all'indice di riga e colonna della cella specificati. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn/)(int) | Ottiene l'elemento [`Column`](../column/) o null all'indice di colonna specificato. |
| [CheckRow](../../aspose.cells/cells/checkrow/)(int) | Ottiene l'elemento [`Row`](../row/) o null all'indice di riga della cella specificato. |
| [Clear](../../aspose.cells/cells/clear/)() | Cancella tutti i dati del foglio di lavoro. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents)(CellArea) | Cancella il contenuto di un range. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents_1)(int, int, int, int) | Cancella il contenuto di un range. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats)(CellArea) | Cancella la formattazione di un range. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats_1)(int, int, int, int) | Cancella la formattazione di un range. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells/)() | Cancella tutti i range uniti. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange)(CellArea) | Cancella il contenuto e la formattazione di un range. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange_1)(int, int, int, int) | Cancella il contenuto e la formattazione di un range. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue/)() | Converte tutti i dati stringa nel foglio di lavoro in valore numerico, se possibile. |
| [CopyColumn](../../aspose.cells/cells/copycolumn/)(Cells, int, int) | Copia i dati e i formati di un'intera colonna. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns)(Cells, int, int, int) | Copia i dati e i formati di intere colonne. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_2)(Cells, int, int, int, int) | Copia i dati e i formati di tutte le colonne. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_1)(Cells, int, int, int, PasteOptions) | Copia i dati e i formati di un'intera colonna. |
| [CopyRow](../../aspose.cells/cells/copyrow/)(Cells, int, int) | Copia i dati e i formati di un'intera riga. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows)(Cells, int, int, int) | Copia i dati e i formati di alcune intere righe. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_1)(Cells, int, int, int, CopyOptions) | Copia i dati e i formati di alcune intere righe. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Copia i dati e i formati di alcune intere righe. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_2)(string) | Crea un oggetto [`Range`](../range/) da un indirizzo dell'intervallo. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_3)(string, string) | Crea un oggetto [`Range`](../range/) da un intervallo di celle. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange)(int, int, bool) | Crea un oggetto [`Range`](../range/) da righe di celle o colonne di celle. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_1)(int, int, int, int) | Crea un oggetto [`Range`](../range/) da un intervallo di celle. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns)() | Elimina tutte le colonne vuote che non contengono alcun dato. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns_1)(DeleteOptions) | Elimina tutte le colonne vuote che non contengono alcun dato. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows)() | Elimina tutte le righe vuote che non contengono alcun dato o altro oggetto. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows_1)(DeleteOptions) | Elimina tutte le righe vuote che non contengono alcun dato o alcuni oggetti speciali come commenti visibili, tabelle pivot. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn)(int) | Elimina una colonna. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn_1)(int, bool) | Elimina una colonna. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns_1)(int, int, bool) | Elimina diverse colonne. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns)(int, int, DeleteOptions) | Elimina diverse colonne. |
| [DeleteRange](../../aspose.cells/cells/deleterange/)(int, int, int, int, ShiftType) | Elimina un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow)(int) | Elimina una riga. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow_1)(int, bool) | Elimina una riga. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows)(int, int) | Elimina più righe. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_2)(int, int, bool) | Elimina più righe nel foglio di lavoro. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_1)(int, int, DeleteOptions) | Elimina più righe nel foglio di lavoro. |
| [Dispose](../../aspose.cells/cells/dispose/)() | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn)(int) | Ottiene l'ultima cella in questa colonna. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn_1)(int, int, int, int) | Ottiene l'ultima cella con indice di colonna massimo in questo intervallo. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow)(int) | Ottiene l'ultima cella in questa riga. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow_1)(int, int, int, int) | Ottiene l'ultima cella con indice di riga massimo in questo intervallo. |
| [ExportArray](../../aspose.cells/cells/exportarray/)(int, int, int, int) | Esporta i dati nella collezione `Cells` in un oggetto array bidimensionale. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable)(int, int, int, int) | Esporta i dati nella collezione `Cells` in un oggetto DataTable. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_2)(int, int, int, int, bool) | Esporta i dati nella collezione `Cells` in un oggetto DataTable. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Esporta i dati nella collezione `Cells` in un oggetto DataTable. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring)(int, int, int, int) | Esporta i dati nella collezione `Cells` in un oggetto DataTable. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring_1)(int, int, int, int, bool) | Esporta i dati nella collezione `Cells` in un oggetto DataTable. |
| [ExportList&lt;T&gt;](../../aspose.cells/cells/exportlist/)(int, int, int, int, ExportTableOptions) |  |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray/)(int, int, int, int) | Esporta il tipo di valore della cella nella collezione `Cells` in un oggetto array bidimensionale. |
| [Find](../../aspose.cells/cells/find/#find)(object, Cell) | Trova la cella contenente l'oggetto di input. |
| [Find](../../aspose.cells/cells/find/#find_1)(object, Cell, FindOptions) | Trova la cella contenente l'oggetto di input. |
| [GetCell](../../aspose.cells/cells/getcell/)(int, int) | (**Obsolete.**) Ottiene l'elemento [`Cell`](../cell/) o null all'indice di riga e colonna della cella specificati. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle)(int, int) | Ottieni lo stile di visualizzazione della cella fornita. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle_1)(int, int, BorderType) | Ottieni lo stile di visualizzazione della cella fornita. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle/)(int, int) | Ottieni lo stile della cella fornita. |
| [GetCellsWithPlaceInCellPicture](../../aspose.cells/cells/getcellswithplaceincellpicture/)() | Restituisce tutte le celle che contengono un'immagine incorporata. |
| [GetColumnOriginalWidthPoint](../../aspose.cells/cells/getcolumnoriginalwidthpoint/)(int) | (**Obsolete.**) Restituisce l'altezza originale della colonna in unità di punto se la colonna è nascosta |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth)(int) | Restituisce la larghezza (in unità di caratteri) della colonna specificata nella visualizzazione normale |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth_1)(int, bool, CellsUnitType) | Restituisce la larghezza della colonna. |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch/)(int) | (**Obsolete.**) Restituisce la larghezza della colonna specificata nella visualizzazione normale, in unità di pollici. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel)(int) | Restituisce la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel_1)(int, bool) | (**Obsolete.**) Restituisce la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel. |
| [GetDependents](../../aspose.cells/cells/getdependents/)(bool, int, int) | Ottieni tutte le celle che fanno riferimento alla cella specifica. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation/)(int, int, bool) | Restituisce tutte le celle il cui risultato calcolato dipende dalla cella specifica. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator/)() | Restituisce l'enumeratore delle celle. |
| [GetFirstDataRow](../../aspose.cells/cells/getfirstdatarow/)(int) | Restituisce l'indice della prima riga della cella che contiene dati nella colonna specificata. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel/)(int) | Restituisce il livello di contorno (basato su zero) della colonna. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel/)(int) | Restituisce il livello di contorno (basato su zero) della riga. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow/)(int) | Restituisce l'indice dell'ultima riga della cella che contiene dati nella colonna specificata. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/)() | Restituisce il livello di contorno massimo delle colonne raggruppate (basato su zero). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel/)() | Restituisce il livello di contorno massimo delle righe raggruppate (basato su zero). |
| [GetMergedAreas](../../aspose.cells/cells/getmergedareas/)() | Restituisce tutte le celle unite. |
| [GetRow](../../aspose.cells/cells/getrow/)(int) | (**Obsolete.**) Restituisce l'elemento [`Row`](../row/) all'indice di riga della cella specificato. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator/)() | (**Obsolete.**) Restituisce l'enumeratore delle righe. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight)(int) | Restituisce l'altezza di una riga specificata, in unità di punti. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight_1)(int, bool, CellsUnitType) | Restituisce l'altezza della riga. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch/)(int) | Restituisce l'altezza di una riga specificata in unità di pollici. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel/)(int) | Restituisce l'altezza di una riga specificata in unità di pixel. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint/)(int) | (**Obsolete.**) Restituisce l'altezza originale della riga in unità di punto se la riga è nascosta |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel/)(int) | Restituisce la larghezza in diversi tipi di visualizzazione. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight/)(int) | Restituisce l'altezza di una riga specificata. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch/)(int) | Restituisce l'altezza di una riga specificata in unità di pollici. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns)(int, int) | Raggruppa le colonne. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns_1)(int, int, bool) | Raggruppa le colonne. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows)(int, int) | Raggruppa le righe. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows_1)(int, int, bool) | Raggruppa le righe. |
| [HideColumn](../../aspose.cells/cells/hidecolumn/)(int) | Nasconde una colonna. |
| [HideColumns](../../aspose.cells/cells/hidecolumns/)(int, int) | Nascondi più colonne. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail/)(bool, int) | Comprimi le righe/colonne raggruppate. |
| [HideRow](../../aspose.cells/cells/hiderow/)(int) | Nasconde una riga. |
| [HideRows](../../aspose.cells/cells/hiderows/)(int, int) | Nasconde più righe. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_1)(double[], int, int, bool) | Importa un array di double in un foglio di lavoro. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_3)(int[], int, int, bool) | Importa un array di integer in un foglio di lavoro. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_5)(string[], int, int, bool) | Importa un array di string in un foglio di lavoro. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist/)(ArrayList, int, int, bool) | Importa un arraylist di dati in un foglio di lavoro. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv)(Stream, TxtLoadOptions, int, int) | Importa un file CSV nelle celle. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_2)(string, TxtLoadOptions, int, int) | Importa un file CSV nelle celle. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_1)(Stream, string, bool, int, int) | Importa un file CSV nelle celle. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_3)(string, string, bool, int, int) | Importa un file CSV nelle celle. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Importa oggetti personalizzati. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Importa oggetti personalizzati. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_3)(IDataReader, int, int) | Importa dati da un oggetto IDataReader. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_1)(DataTable, int, int, ImportTableOptions) | Importa dati da una tabella dati personalizzata. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_2)(DataView, int, int, ImportTableOptions) | Importa dati da una vista dati. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Importa dati da una tabella dati personalizzata. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_4)(IDataReader, int, int, ImportTableOptions) | Importa dati da un oggetto IDataReader. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid)(DataGrid, int, int, bool) | Importa un DataGrid in un foglio di lavoro. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Importa un DataGrid in un foglio di lavoro. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Importa un DataGrid in un foglio di lavoro. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring/)(DataGrid, int, int, bool) | Importa un DataGrid in un foglio di lavoro. Questo metodo non tenta di convertire il testo in valori numerici. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow/)(DataRow, int, int) | Importa un DataRow nel file Excel. |
| [ImportDataView](../../aspose.cells/cells/importdataview/)(DataView, int, int) | Importa un DataView in un foglio di lavoro. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray/)(string[], int, int, bool) | Importa un array di formula in un foglio di lavoro. |
| [ImportGridView](../../aspose.cells/cells/importgridview/)(GridView, int, int, ImportTableOptions) | Importa una visualizzazione a griglia in queste celle. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray)(object[], int, int, bool) | Importa un array di dati in un foglio di lavoro. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray_1)(object[], int, int, bool, int) | Importa un array di dati in un foglio di lavoro. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn)(int) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn_1)(int, bool) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns)(int, int) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_2)(int, int, bool) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_1)(int, int, InsertOptions) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells/)(Range, int, int, ShiftType) | Inserisci intervallo tagliato. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange)(CellArea, ShiftType) | Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_1)(CellArea, int, ShiftType) | Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_2)(CellArea, int, ShiftType, bool) | Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [InsertRow](../../aspose.cells/cells/insertrow/)(int) | Inserisce una nuova riga nel foglio di lavoro. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows)(int, int) | Inserisce più righe nel foglio di lavoro. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_2)(int, int, bool) | Inserisce più righe nel foglio di lavoro. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_1)(int, int, InsertOptions) | Inserisce più righe nel foglio di lavoro. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn/)(int) | Verifica se la colonna specificata è vuota (non contiene alcun dato). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden/)(int) | Verifica se una colonna all'indice specificato è nascosta. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled/)(int, int, int, int) | Verifica se l'intervallo può essere eliminato. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden/)(int) | Verifica se una riga all'indice specificato è nascosta. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap/)(string, int, int, string) | Collegamento a una mappa XML. |
| [Merge](../../aspose.cells/cells/merge/#merge)(int, int, int, int) | Unisce un intervallo di celle specificato in un'unica cella. |
| [Merge](../../aspose.cells/cells/merge/#merge_1)(int, int, int, int, bool) | Unisce un intervallo di celle specificato in un'unica cella. |
| [Merge](../../aspose.cells/cells/merge/#merge_2)(int, int, int, int, bool, bool) | Unisce un intervallo di celle specificato in un'unica cella. |
| [MoveRange](../../aspose.cells/cells/moverange/)(CellArea, int, int) | Sposta l'intervallo. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates)() | Rimuove le righe duplicate nel foglio. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_1)(int, int, int, int) | Rimuove i valori duplicati nell'intervallo. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_2)(int, int, int, int, bool, int[]) | Rimuove i dati duplicati dell'intervallo. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas/)() | Rimuove tutte le formule e le sostituisce con il valore della formula. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting/)(CellArea) | Recupera le impostazioni dei subtotali dell'intervallo. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth/)(int, double) | Imposta la larghezza della colonna specificata nella visualizzazione normale. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch/)(int, double) | Imposta la larghezza della colonna in unità di pollici nella visualizzazione normale. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel/)(int, int) | Imposta la larghezza della colonna in unità di pixel nella visualizzazione normale. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight/)(int, double) | Imposta l'altezza della riga specificata. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch/)(int, double) | Imposta l'altezza della riga in unità di pollici. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel/)(int, int) | Imposta l'altezza della riga in unità di pixel. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel/)(int, int) | Imposta la larghezza della colonna in visualizzazioni diverse. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail/)(bool, int) | Espande le righe/colonne raggruppate. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Crea subtotali per l'intervallo. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Crea subtotali per l'intervallo. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns/)(int, int, int, TxtLoadOptions) | Divide il contenuto nella colonna specificata in più colonne.. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns/)(int, int) | Separa le colonne dal raggruppamento. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows)(int, int) | Separa le righe dal raggruppamento. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows_1)(int, int, bool) | Separa le righe dal raggruppamento. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn/)(int, double) | Rende visibile una colonna |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns/)(int, int, double) | Rende visibili più colonne. |
| [UnhideRow](../../aspose.cells/cells/unhiderow/)(int, double) | Rende visibile una riga. |
| [UnhideRows](../../aspose.cells/cells/unhiderows/)(int, int, double) | Rende visibili le righe nascoste. |
| [UnMerge](../../aspose.cells/cells/unmerge/)(int, int, int, int) | Separa un intervallo specificato di celle unite. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDemo
    {
        public static void CellsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta l'altezza predefinita della riga
            cells.StandardHeight = 20;
            // Imposta l'altezza della riga
            cells.SetRowHeight(2, 20.5);

            // Imposta la larghezza predefinita della colonna
            cells.StandardWidth = 15;
            // Imposta la larghezza della colonna
            cells.SetColumnWidth(3, 12.57);

            // Unisci le celle
            cells.Merge(5, 4, 2, 2);

            // Inserisci valori nelle celle
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(1);
            cells[0, 2].PutValue("abc");

            // Esporta dati
            object[,] arr = cells.ExportArray(0, 0, 10, 10);

            // Dimostra alcune proprietà
            Console.WriteLine("Total Cells Count: " + cells.Count);
            Console.WriteLine("Total Cells Count (Large): " + cells.CountLarge);
            Console.WriteLine("Min Row with Data: " + cells.MinDataRow);
            Console.WriteLine("Max Row with Data: " + cells.MaxDataRow);
            Console.WriteLine("Min Column with Data: " + cells.MinDataColumn);
            Console.WriteLine("Max Column with Data: " + cells.MaxDataColumn);

            // Itera attraverso le celle
            IEnumerator enumerator = cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Salva la cartella di lavoro
            workbook.Save("CellsExample.xlsx");
            workbook.Save("CellsExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


