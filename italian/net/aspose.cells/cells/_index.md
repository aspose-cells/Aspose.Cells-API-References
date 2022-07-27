---
title: Cells
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula una raccolta di oggetti rilevanti per la cella comeCell./cell Row./row ...ecc.
type: docs
weight: 300
url: /it/net/aspose.cells/cells/
---
## Cells class

Incapsula una raccolta di oggetti rilevanti per la cella, come[`Cell`](../cell) ,[`Row`](../row) ...ecc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns) { get; } | Ottiene la raccolta di[`Column`](../column) oggetti che rappresentano le singole colonne in questo foglio di lavoro. |
| [Count](../../aspose.cells/cells/count) { get; } | Ottiene il conteggio totale degli oggetti Cell istanziati. |
| [CountLarge](../../aspose.cells/cells/countlarge) { get; } | Ottiene il conteggio totale degli oggetti Cell istanziati. |
| [FirstCell](../../aspose.cells/cells/firstcell) { get; } | Ottiene la prima cella in questo foglio di lavoro. |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched) { get; set; } | Indica che l'altezza della riga e l'altezza del carattere predefinita corrispondono a |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden) { get; set; } | Indica se la riga è nascosta per impostazione predefinita. |
| [Item](../../aspose.cells/cells/item) { get; } | Ottiene il[`Cell`](../cell) elemento in corrispondenza dell'indice di riga della cella e dell'indice di colonna specificati. (2 indexers) |
| [LastCell](../../aspose.cells/cells/lastcell) { get; } | Ottiene l'ultima cella in questo foglio di lavoro. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn) { get; } | Indice di colonna minimo di quelle celle di cui è stata creata un'istanza nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma in essa non è stata istanziata alcuna cella). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn) { get; } | Indice di colonna massimo della cella che contiene dati. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow) { get; } | Indice di riga massimo della cella che contiene dati. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange) { get; } | Ottiene l'intervallo massimo che include dati, celle e forme unite. |
| [MaxRow](../../aspose.cells/cells/maxrow) { get; } | Indice di riga massimo della cella che contiene dati o stile. |
| [MemorySetting](../../aspose.cells/cells/memorysetting) { get; set; } | Ottiene o imposta l'opzione di utilizzo della memoria per queste celle. |
| [MergedCells](../../aspose.cells/cells/mergedcells) { get; } | Ottiene la raccolta di celle unite. |
| [MinColumn](../../aspose.cells/cells/mincolumn) { get; } | Indice di colonna minimo di quelle celle di cui è stata creata un'istanza nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma in essa non è stata istanziata alcuna cella). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn) { get; } | Indice di colonna minimo della cella che contiene dati. |
| [MinDataRow](../../aspose.cells/cells/mindatarow) { get; } | Indice di riga minimo della cella che contiene dati. |
| [MinRow](../../aspose.cells/cells/minrow) { get; } | Indice di riga minimo della cella che contiene dati o stile. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading) { get; set; } | Ottiene o imposta se il modello di dati delle celle deve supportare la lettura multi-thread. Il valore predefinito di questa proprietà è false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields) { get; } | Ottiene l'elenco dei campi di ods. |
| [PreserveString](../../aspose.cells/cells/preservestring) { get; set; } | Ottiene o imposta un valore che indica se tutti i valori del foglio di lavoro vengono mantenuti come stringhe. L'impostazione predefinita è false. |
| [Ranges](../../aspose.cells/cells/ranges) { get; } | Ottiene la raccolta di[`Range`](../range)oggetti creati in fase di esecuzione. |
| [Rows](../../aspose.cells/cells/rows) { get; } | Ottiene la raccolta di[`Row`](../row) oggetti che rappresentano le singole righe in questo foglio di lavoro. |
| [StandardHeight](../../aspose.cells/cells/standardheight) { get; set; } | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di punti. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch) { get; set; } | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di pollici. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels) { get; set; } | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di pixel. |
| [StandardWidth](../../aspose.cells/cells/standardwidth) { get; set; } | Ottiene o imposta la larghezza della colonna predefinita nel foglio di lavoro, in unità di caratteri. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch) { get; set; } | Ottiene o imposta la larghezza della colonna predefinita nel foglio di lavoro, in unità di pollici. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels) { get; set; } | Ottiene o imposta la larghezza della colonna predefinita nel foglio di lavoro, in unità di pixel. |
| [Style](../../aspose.cells/cells/style) { get; set; } | Ottiene e imposta lo stile predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange)(Range) | Aggiunge un riferimento all'oggetto intervallo alle celle |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle)(int, Style, StyleFlag) | Applica i formati per un'intera colonna. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle)(int, Style, StyleFlag) | Applica i formati per un'intera riga. |
| [ApplyStyle](../../aspose.cells/cells/applystyle)(Style, StyleFlag) | Applica i formati per un intero foglio di lavoro. |
| [CheckCell](../../aspose.cells/cells/checkcell)(int, int) | Ottiene il[`Cell`](../cell) elemento o null in corrispondenza dell'indice di riga della cella e dell'indice di colonna specificati. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn)(int) | Ottiene il[`Column`](../column) elemento o null in corrispondenza dell'indice di colonna specificato. |
| [CheckRow](../../aspose.cells/cells/checkrow)(int) | Ottiene il[`Row`](../row) elemento o all'indice della riga della cella specificato. |
| [Clear](../../aspose.cells/cells/clear)() | Cancella tutti gli oggetti cella e riga. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents)(CellArea) | Cancella il contenuto di un intervallo. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents_1)(int, int, int, int) | Cancella il contenuto di un intervallo. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats)(CellArea) | Cancella la formattazione di un intervallo. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats_1)(int, int, int, int) | Cancella la formattazione di un intervallo. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells)() | Cancella tutti gli intervalli uniti. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange)(CellArea) | Cancella il contenuto e la formattazione di un intervallo. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange_1)(int, int, int, int) | Cancella il contenuto e la formattazione di un intervallo. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue)() | Converte i dati della stringa nelle celle in un valore numerico, se possibile. |
| [CopyColumn](../../aspose.cells/cells/copycolumn)(Cells, int, int) | Copia dati e formati di un'intera colonna. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns)(Cells, int, int, int) | Copia dati e formati di un'intera colonna. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_2)(Cells, int, int, int, int) | Copia dati e formati di intere colonne. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_1)(Cells, int, int, int, PasteOptions) | Copia dati e formati di un'intera colonna. |
| [CopyRow](../../aspose.cells/cells/copyrow)(Cells, int, int) | Copia dati e formati di un'intera riga. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows)(Cells, int, int, int) | Copia i dati e i formati di alcune righe intere. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_1)(Cells, int, int, int, CopyOptions) | Copia i dati e i formati di alcune righe intere. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Copia i dati e i formati di alcune righe intere. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_2)(string) | Crea a[`Range`](../range) oggetto da un indirizzo dell'intervallo. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_3)(string, string) | Crea a[`Range`](../range) oggetto da un intervallo di celle. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange)(int, int, bool) | Crea a[`Range`](../range) oggetto da righe di celle o colonne di celle. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_1)(int, int, int, int) | Crea a[`Range`](../range) oggetto da un intervallo di celle. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns)() | Elimina tutte le colonne vuote che non contengono dati. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns_1)(DeleteOptions) | Elimina tutte le colonne vuote che non contengono dati. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows)() | Elimina tutte le righe vuote che non contengono dati. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows_1)(DeleteOptions) | Elimina tutte le righe vuote che non contengono dati. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn)(int) | Elimina una colonna. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn_1)(int, bool) | Elimina una colonna. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns)(int, int, bool) | Elimina diverse colonne. |
| [DeleteRange](../../aspose.cells/cells/deleterange)(int, int, int, int, ShiftType) | Elimina un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [DeleteRow](../../aspose.cells/cells/deleterow)(int) | Elimina una riga. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows)(int, int) | Elimina diverse righe. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows_1)(int, int, bool) | Elimina più righe nel foglio di lavoro. |
| [Dispose](../../aspose.cells/cells/dispose)() | Esegue attività definite dall'applicazione associate alla liberazione, rilascio o ripristino di risorse non gestite. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn)(short) | Ottiene l'ultima cella in questa colonna. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn_1)(int, int, short, short) | Ottiene l'ultima cella con indice di colonna massimo in questo intervallo. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow)(int) | Ottiene l'ultima cella di questa riga. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow_1)(int, int, int, int) | Ottiene l'ultima cella con il massimo indice di riga in questo intervallo. |
| [ExportArray](../../aspose.cells/cells/exportarray)(int, int, int, int) | Esporta i dati nel file[`Cells`](../cells) raccolta in un oggetto array a due dimensioni. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable)(int, int, int, int) | Esporta i dati nel file[`Cells`](../cells) raccolta ad aDataTable oggetto. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_2)(int, int, int, int, bool) | Esporta i dati nel file[`Cells`](../cells) raccolta ad aDataTable oggetto. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Esporta i dati nel file[`Cells`](../cells) raccolta ad aDataTable oggetto. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring)(int, int, int, int) | Esporta i dati nel file[`Cells`](../cells) raccolta ad aDataTable oggetto. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring_1)(int, int, int, int, bool) | Esporta i dati nel file[`Cells`](../cells) raccolta ad aDataTable oggetto. |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray)(int, int, int, int) | Esporta il tipo di valore della cella nel file[`Cells`](../cells) raccolta in un oggetto array a due dimensioni. |
| [Find](../../aspose.cells/cells/find#find)(object, Cell) | Trova la cella contenente con l'oggetto di input. |
| [Find](../../aspose.cells/cells/find#find_1)(object, Cell, FindOptions) | Trova la cella contenente con l'oggetto di input. |
| [GetCell](../../aspose.cells/cells/getcell)(int, int) | Ottiene il[`Cell`](../cell) elemento o null in corrispondenza dell'indice di riga della cella e dell'indice di colonna specificati. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle)(int, int) | Ottieni lo stile della cella data. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth)(int) | Ottiene la larghezza della colonna specificata nella vista normale |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch)(int) | Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pollici. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel)(int) | Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel. |
| [GetDependents](../../aspose.cells/cells/getdependents)(bool, int, int) | Ottieni tutte le celle che fanno riferimento alla cella specifica. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation)(int, int, bool) | Ottiene tutte le celle il cui risultato calcolato dipende da una cella specifica. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator)() | Ottiene l'enumeratore di celle. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel)(int) | Ottiene il livello di struttura (in base zero) della colonna. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel)(int) | Ottiene il livello di struttura (in base zero) della riga. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow)(int) | Ottiene l'ultimo indice di riga della cella che contiene i dati nella colonna specificata. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel)() | Ottiene il livello massimo di struttura della colonna raggruppata (a base zero). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel)() | Ottiene il livello massimo di struttura delle righe raggruppate (a base zero). |
| [GetRow](../../aspose.cells/cells/getrow)(int) | Ottiene il[`Row`](../row) elemento all'indice della riga della cella specificato. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator)() | Ottiene l'enumeratore di righe. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight)(int) | Ottiene l'altezza di una riga specificata. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch)(int) | Ottiene l'altezza di una riga specificata in unità di pollici. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel)(int) | Ottiene l'altezza di una riga specificata in unità di pixel. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint)(int) | Ottiene l'altezza della riga originale in unità di punto se la riga è nascosta |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel)(int) | Ottieni la larghezza in un diverso tipo di vista. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight)(int) | Ottiene l'altezza di una riga specificata. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch)(int) | Ottiene l'altezza di una riga specificata in unità di pollici. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns)(int, int) | Colonne dei gruppi. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns_1)(int, int, bool) | Colonne dei gruppi. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows)(int, int) | Raggruppa righe. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows_1)(int, int, bool) | Raggruppa righe. |
| [HideColumn](../../aspose.cells/cells/hidecolumn)(int) | Nasconde una colonna. |
| [HideColumns](../../aspose.cells/cells/hidecolumns)(int, int) | Nascondi più colonne. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail)(bool, int) | Comprime le righe/colonne raggruppate. |
| [HideRow](../../aspose.cells/cells/hiderow)(int) | Nasconde una riga. |
| [HideRows](../../aspose.cells/cells/hiderows)(int, int) | Nasconde più righe. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_1)(double[], int, int, bool) | Importa un array di double in un foglio di lavoro. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_3)(int[], int, int, bool) | Importa una matrice di numeri interi in un foglio di lavoro. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_5)(string[], int, int, bool) | Importa una matrice di stringhe in un foglio di lavoro. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist)(ArrayList, int, int, bool) | Importa un arraylist di dati in un foglio di lavoro. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv)(Stream, TxtLoadOptions, int, int) | Importa un file CSV nelle celle. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_2)(string, TxtLoadOptions, int, int) | Importa un file CSV nelle celle. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_1)(Stream, string, bool, int, int) | Importa un file CSV nelle celle. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_3)(string, string, bool, int, int) | Importa un file CSV nelle celle. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Importa oggetti personalizzati. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Importa oggetti personalizzati. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_3)(IDataReader, int, int) | Importa i dati da aIDataReader oggetto. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_1)(DataTable, int, int, ImportTableOptions) | Importa dati dalla tabella dati personalizzata. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_2)(DataView, int, int, ImportTableOptions) | Importa dati dalla visualizzazione dati. |
| [ImportData](../../aspose.cells/cells/importdata#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Importa dati dalla tabella dati personalizzata. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_4)(IDataReader, int, int, ImportTableOptions) | Importa i dati da aIDataReader oggetto. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid)(DataGrid, int, int, bool) | Importazioni aDataGrid in un foglio di lavoro. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Importazioni aDataGrid in un foglio di lavoro. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Importazioni aDataGrid in un foglio di lavoro. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring)(DataGrid, int, int, bool) | Importazioni aDataGrid in un foglio di lavoro. Questo metodo non tenta di convertire il testo in valori numerici. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow)(DataRow, int, int) | Importa una DataRow nel file Excel. |
| [ImportDataView](../../aspose.cells/cells/importdataview#importdataview_3)(DataView, int, int) | Importazioni aDataView in un foglio di lavoro. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray)(string[], int, int, bool) | Importa una matrice di formule in un foglio di lavoro. |
| [ImportGridView](../../aspose.cells/cells/importgridview)(GridView, int, int, ImportTableOptions) | Importa una vista griglia in queste celle. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray)(object[], int, int, bool) | Importa una matrice di dati in un foglio di lavoro. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray_1)(object[], int, int, bool, int) | Importa una matrice di dati in un foglio di lavoro. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn)(int) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn_1)(int, bool) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns)(int, int) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns_1)(int, int, bool) | Inserisce alcune colonne nel foglio di lavoro. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells)(Range, int, int, ShiftType) | Inserisci intervallo di taglio. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange)(CellArea, ShiftType) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_1)(CellArea, int, ShiftType) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_2)(CellArea, int, ShiftType, bool) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [InsertRow](../../aspose.cells/cells/insertrow)(int) | Inserisce una nuova riga nel foglio di lavoro. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows)(int, int) | Inserisce più righe nel foglio di lavoro. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_2)(int, int, bool) | Inserisce più righe nel foglio di lavoro. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_1)(int, int, InsertOptions) | Inserisce più righe nel foglio di lavoro. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn)(int) | Verifica se la colonna data è vuota (non contiene dati). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden)(int) | Verifica se una colonna in un determinato indice è nascosta. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled)(int, int, int, int) | Verifica se l'intervallo può essere eliminato. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden)(int) | Verifica se una riga in un determinato indice è nascosta. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap)(string, int, int, string) | Collegamento a una mappa xml. |
| [Merge](../../aspose.cells/cells/merge#merge)(int, int, int, int) | Unisce un intervallo di celle specificato in una singola cella. |
| [Merge](../../aspose.cells/cells/merge#merge_1)(int, int, int, int, bool) | Unisce un intervallo di celle specificato in una singola cella. |
| [Merge](../../aspose.cells/cells/merge#merge_2)(int, int, int, int, bool, bool) | Unisce un intervallo di celle specificato in una singola cella. |
| [MoveRange](../../aspose.cells/cells/moverange)(CellArea, int, int) | Sposta l'intervallo. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates)() | Rimuove le righe duplicate nel foglio. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_1)(int, int, int, int) | Rimuove i valori duplicati nell'intervallo. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_2)(int, int, int, int, bool, int[]) | Rimuove i dati duplicati dell'intervallo. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas)() | Rimuove tutta la formula e la sostituisce con il valore della formula. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting)(CellArea) | Recupera l'impostazione dei totali parziali dell'intervallo. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth)(int, double) | Imposta la larghezza della colonna specificata nella vista normale. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch)(int, double) | Imposta la larghezza della colonna in unità di pollici nella vista normale. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel)(int, int) | Imposta la larghezza della colonna in unità di pixel nella vista normale. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight)(int, double) | Imposta l'altezza della riga specificata. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch)(int, double) | Imposta l'altezza della riga in unità di pollici. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel)(int, int) | Imposta l'altezza della riga in unità di pixel. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel)(int, int) | Imposta la larghezza della colonna in una vista diversa. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail)(bool, int) | Espande le righe/colonne raggruppate. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Crea i totali parziali per l'intervallo. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Crea i totali parziali per l'intervallo. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns)(int, int, int, TxtLoadOptions) | Divide il testo nella colonna in colonne. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns)(int, int) | Separa le colonne. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows)(int, int) | Separa le righe. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows_1)(int, int, bool) | Separa le righe. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn)(int, double) | Mostra una colonna |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns)(int, int, double) | Mostra più colonne. |
| [UnhideRow](../../aspose.cells/cells/unhiderow)(int, double) | Mostra una riga. |
| [UnhideRows](../../aspose.cells/cells/unhiderows)(int, int, double) | Mostra le righe nascoste. |
| [UnMerge](../../aspose.cells/cells/unmerge)(int, int, int, int) | Separa un intervallo specificato di celle unite. |

### Esempi

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Imposta l'altezza della riga predefinita
cells.StandardHeight = 20;
//Imposta l'altezza della riga
cells.SetRowHeight(2, 20.5);

//Imposta la larghezza della colonna predefinita
cells.StandardWidth = 15;
//Imposta la larghezza della colonna
cells.SetColumnWidth(3, 12.57);

//Unire le celle
cells.Merge(5, 4, 2, 2);

//Inserisce i valori nelle celle
cells[0, 0].PutValue(true);
cells[0, 1].PutValue(1);
cells[0, 2].PutValue("abc");

//Esporta dati
object[,] arr = cells.ExportArray(0, 0, 10, 10);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Imposta l'altezza della riga predefinita
cells.StandardHeight = 20
'Imposta l'altezza della riga
cells.SetRowHeight(2, 20.5)

'Imposta la larghezza della colonna predefinita
cells.StandardWidth = 15
'Imposta la larghezza della colonna
cells.SetColumnWidth(3, 12.57)

'Unire le celle
cells.Merge(5, 4, 2, 2)

'Esporta dati
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
