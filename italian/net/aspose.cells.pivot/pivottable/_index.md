---
title: PivotTable
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Descrizione riepilogativa per tabella pivot.
type: docs
weight: 4690
url: /it/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Descrizione riepilogativa per tabella pivot.

```csharp
public class PivotTable : IDisposable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription) { get; set; } | Ottiene la descrizione del testo alternativo |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle) { get; set; } | Ottiene il titolo dell'altertext |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype) { get; set; } | Ottiene il tipo di formato automatico della tabella pivot. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields) { get; } | Restituisce un oggetto PivotFields che include tutti i campi nel report tabella pivot |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields) { get; } | Restituisce un oggetto PivotFields che è attualmente mostrato come campi colonna. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand) { get; set; } | Indica se il rapporto tabella pivot mostra i totali complessivi per le colonne. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption) { get; set; } | Ottiene la didascalia dell'intestazione della colonna della tabella pivot. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange) { get; } | Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area della colonna nel report di tabella pivot. Sola lettura. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort) { get; set; } | Indica se considerare l'elenco personalizzato integrato quando si ordinano i dati |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange) { get; } | Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area dati nell'elenco tra la riga di intestazione e la riga di inserimento. Sola lettura. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield) { get; } | Ottiene un oggetto PivotField che rappresenta tutti i campi di dati in una tabella pivot. Sola lettura. Sarebbe init solo quando sono presenti due o più campi di dati in DataPiovtFiels. Viene utilizzato solo per aggiungere DataPivotField alla riga/colonna della tabella pivot la zona . L'impostazione predefinita è nell'area della riga. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields) { get; } | Ottiene un oggetto PivotField che rappresenta tutti i campi di dati in una tabella pivot. Sola lettura. Sarebbe init solo quando sono presenti due o più campi di dati in DataPiovtFiels. Viene utilizzato solo per aggiungere DataPivotField alla riga/colonna della tabella pivot la zona . L'impostazione predefinita è nell'area della riga. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource) { get; set; } | Ottiene e imposta l'origine dati della tabella pivot. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring) { get; set; } | Indica se il report di tabella pivot visualizza una stringa personalizzata nelle celle che contengono errori. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems) { get; set; } | Indica se gli elementi nelle aree di riga e colonna sono visibili quando l'area dati della tabella pivot è vuota. Il valore predefinito è true. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring) { get; set; } | Indica se il report di tabella pivot visualizza una stringa personalizzata nelle celle che contengono valori Null. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting) { get; set; } | Specifica un valore booleano che indica se l'utente è autorizzato a modificare le celle nell'area dati della tabella pivot. Abilita la modifica delle celle nell'area dei valori |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown) { get; set; } | Ottiene se il drilldown è abilitato. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog) { get; set; } | Indica se la finestra di dialogo Campo tabella pivot è disponibile quando l'utente fa doppio clic sul campo tabella pivot. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist) { get; set; } | Ottiene se abilitare l'elenco dei campi per la tabella pivot. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard) { get; set; } | Indica se la procedura guidata tabella pivot è disponibile. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring) { get; set; } | Ottiene la stringa visualizzata nelle celle che contengono errori quando la proprietà DisplayErrorString è true. Il valore predefinito è una stringa vuota. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource) { get; } | Ottiene l'origine dati della connessione esterna. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending) { get; set; } | Specifica un valore booleano che indica se i campi della tabella pivot sono ordinati in un ordine non predefinito nell'elenco dei campi. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname) { get; set; } | Restituisce l'etichetta della stringa di testo visualizzata nella colonna o nell'intestazione della riga del totale generale. Il valore predefinito è la stringa "Totale generale". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows) { get; set; } | Indica se aggiungere righe vuote. Questa proprietà si applica solo ai tipi di formato automatico della tabella pivot che devono aggiungere righe vuote. |
| [Indent](../../aspose.cells.pivot/pivottable/indent) { get; set; } | Specifica l'incremento di rientro per l'asse compatto e può essere utilizzato per impostare il layout del report su Compact Form. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat) { get; set; } | Indica se il report della tabella pivot viene formattato automaticamente. Casella di controllo "formattazione automatica tabella" che è nell'opzione pivottable per Excel 2003 Casella di controllo "adatta larghezza colonna all'aggiornamento" che si trova nella tabella pivot Opzioni: Formato layout per Excel 2007 |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible) { get; set; } | Specifica se la tabella pivot è compatibile con Excel2003 durante l'aggiornamento della tabella pivot, se true, una stringa deve essere minore o uguale a 255 caratteri, quindi se la stringa è maggiore di 255 caratteri, verrà troncata. se false, una stringa non avrà la suddetta limitazione. Il valore predefinito è true. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones) { get; set; } | Indica se il report di tabella pivot visualizza il layout pivottable classico. (abilita il trascinamento dei campi nella griglia) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters) { get; set; } | Specifica un valore booleano che indica se i campi di una tabella pivot possono avere più filtri impostati su di essi. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected) { get; set; } | Indica se la tabella pivot è selezionata. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles) { get; set; } | Un bit che specifica se le didascalie degli elementi pivot sull'asse della riga vengono ripetute su ogni pagina stampata per i campi pivot in forma tabellare. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate) { get; set; } | Indica se il report della tabella pivot viene ricalcolato solo su richiesta dell'utente. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels) { get; set; } | Indica se le etichette dell'elemento della riga esterna, dell'elemento della colonna, del subtotale, e del totale generale del rapporto tabella pivot specificati utilizzano celle unite. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit) { get; set; } | Specifica un valore booleano che indica se i campi di una tabella pivot possono avere più filtri impostati su di essi. |
| [Name](../../aspose.cells.pivot/pivottable/name) { get; set; } | Ottiene il nome della tabella pivot |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring) { get; set; } | Ottiene la stringa visualizzata nelle celle che contengono valori Null quando la proprietà DisplayNullString è true. Il valore predefinito è una stringa vuota. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder) { get; set; } | Ottiene l'ordine in cui i campi della pagina vengono aggiunti al layout del report della tabella pivot. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields) { get; } | Restituisce un oggetto PivotFields che è attualmente mostrato come campi di pagina. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount) { get; set; } | Ottiene il numero di campi di pagina in ogni colonna o riga nel report di tabella pivot. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters) { get; } | Restituisce un oggetto PivotFilterCollection. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions) { get; } | Ottiene le condizioni di formato della tabella pivot. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename) { get; set; } | Ottiene e imposta il nome dello stile pivottable. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype) { get; set; } | Ottiene e imposta lo stile della tabella pivot integrato. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting) { get; set; } | Indica se la formattazione viene conservata quando la tabella pivot viene aggiornata o ricalcolata. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill) { get; set; } | Specifica un valore booleano che indica se devono essere stampati gli indicatori di drill. stampa pulsanti di espansione/compressione quando visualizzati su pivottable. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles) { get; set; } | Indica se i titoli di stampa per il foglio di lavoro sono impostati in base a sul report della tabella pivot. Il valore predefinito è false. |
| [RefreshDataFlag](../../aspose.cells.pivot/pivottable/refreshdataflag) { get; set; } | Indica se Aggiorna i dati o meno. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile) { get; set; } | Indica se Aggiorna i dati all'apertura del file. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate) { get; } | Ottiene la data dell'ultimo aggiornamento della tabella pivot. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho) { get; } | Ottiene il nome dell'utente che ha aggiornato per ultimo la tabella pivot |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields) { get; } | Restituisce un oggetto PivotFields che è attualmente mostrato come campi riga. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand) { get; set; } | Indica se il rapporto tabella pivot mostra i totali complessivi per le righe. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption) { get; set; } | Ottiene la didascalia dell'intestazione di riga della tabella pivot. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange) { get; } | Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area della riga nel report di tabella pivot. Sola lettura. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata) { get; set; } | Indica se i dati per il report della tabella pivot vengono salvati con la cartella di lavoro. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips) { get; set; } | Specifica un valore booleano che indica se le descrizioni comandi devono essere visualizzate per le celle di dati della tabella pivot. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill) { get; set; } | Ottiene se vengono visualizzati i pulsanti di espansione/compressione. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol) { get; set; } | Specifica un valore booleano che indica se includere colonne vuote nella tabella |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow) { get; set; } | Specifica un valore booleano che indica se includere righe vuote nella tabella. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips) { get; set; } | Specifica un valore booleano che indica se le informazioni sulla proprietà del membro devono essere omesse dalle descrizioni comandi della tabella pivot. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader) { get; set; } | Indica se l'intestazione della colonna nella tabella pivot deve avere lo stile applicato. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes) { get; set; } | Indica se è stata applicata la formattazione della striscia di colonna. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn) { get; set; } | Indica se è stata applicata la formattazione della striscia di colonna. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader) { get; set; } | Indica se l'intestazione di riga nella tabella pivot deve avere lo stile applicato. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes) { get; set; } | Indica se è stata applicata la formattazione della striscia di riga. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption) { get; set; } | Indica se la didascalia dell'intestazione di riga è mostrata nel report della tabella pivot Indica se Visualizza le didascalie dei campi e i filtri a discesa |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow) { get; set; } | Specifica un valore booleano che indica se mostrare i valori riga. mostrare i valori riga |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems) { get; set; } | Indica se gli elementi dei campi pagina nascosti nel rapporto tabella pivot sono inclusi nei totali parziali di righe e colonne, nei totali dei blocchi e nei totali complessivi. Il valore predefinito è False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1) { get; } | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report di tabella pivot, ma non include i campi della pagina. Sola lettura. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2) { get; } | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report di tabella pivot, include i campi della pagina. Sola lettura. |
| [Tag](../../aspose.cells.pivot/pivottable/tag) { get; set; } | Ottiene una stringa salvata con il rapporto tabella pivot. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield)(string, string) | Aggiunge un campo calcolato al campo pivot e trascinalo nell'area dati. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield_1)(string, string, bool) | Aggiunge un campo calcolato al campo pivot. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_1)(PivotFieldType, int) | Aggiunge il campo all'area specifica. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea)(PivotFieldType, PivotField) | Aggiunge il campo all'area specifica. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_2)(PivotFieldType, string) | Aggiunge il campo all'area specifica. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata)() | Calcola i dati di pivottable nelle celle. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange)() | Calcola l'intervallo della tabella pivot. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource)(string[]) | Imposta i dati di origine della tabella pivot. Foglio1!$A$1:$C$3 |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata)() | Cancella i dati e la formattazione della tabella pivot |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle)(PivotTable) | Copia lo stile denominato da un'altra tabella pivot. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose)() | Esegue attività definite dall'applicazione associate alla liberazione, rilascio o ripristino di risorse non gestite. |
| [Fields](../../aspose.cells.pivot/pivottable/fields)(PivotFieldType) | Ottiene i campi specifici in base al tipo di campo. |
| [Format](../../aspose.cells.pivot/pivottable/format)(int, int, Style) | Formatta la cella nell'area pivottable |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall)(Style) | Formatta tutta la cella nell'area pivottable |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow)(int, Style) | Formatta i dati della riga nell'area pivottable |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname)(string) | Ottiene l'oggetto Cell da DisplayName di PivotField |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren)() | Ottiene le tabelle pivot figli che utilizzano i dati di questa tabella pivot come origine dati. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks)() | ottieni l'elenco dell'indice delle righe della tabella pivot di interruzioni di pagina orizzontali |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource)() | Ottieni i dati di origine di pivottable. |
| [Move](../../aspose.cells.pivot/pivottable/move#move_1)(string) | Sposta la tabella pivot in una posizione diversa nel foglio di lavoro. |
| [Move](../../aspose.cells.pivot/pivottable/move#move)(int, int) | Sposta la tabella pivot in una posizione diversa nel foglio di lavoro. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata)() | Aggiorna i dati e le impostazioni di pivottable dalla sua origine dati. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_1)(PivotFieldType, int) | Rimuove un campo da un'area di campo specifica |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield)(PivotFieldType, PivotField) | Rimuovi campo dall'area campo specifica |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_2)(PivotFieldType, string) | Rimuove un campo da un'area di campo specifica |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield_1)(int) | Imposta il gruppo di campi automatici in base alla tabella pivot. |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield)(PivotField) | Imposta il gruppo di campi automatici in base alla tabella pivot. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_3)(int, DateTime, DateTime, ArrayList, int) | Imposta il gruppo di campi manuale dalla tabella pivot. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_2)(int, double, double, ArrayList, double) | Imposta il gruppo di campi manuale dalla tabella pivot. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_1)(PivotField, DateTime, DateTime, ArrayList, int) | Imposta il gruppo di campi manuale dalla tabella pivot. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield)(PivotField, double, double, ArrayList, double) | Imposta il gruppo di campi manuale dalla tabella pivot. |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup_1)(int) | Imposta la separazione dalla tabella pivot |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup)(PivotField) | Imposta la separazione dalla tabella pivot |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform)() | Dispone la tabella pivot in forma compatta. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform)() | Dispone la tabella pivot sotto forma di struttura. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform)() | Dispone la tabella pivot in forma tabellare. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage)(PivotField) | Mostra tutte le pagine dei filtri dei report in base a PivotField, il PivotField deve trovarsi nei PageField. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex)(int) | Mostra tutte le pagine dei filtri dei report in base all'indice di posizione nei PageFields |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname)(string) | Mostra tutte le pagine dei filtri dei report in base al nome di PivotField, il PivotField deve trovarsi nei PageField. |

### Esempi

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Modifica gli attributi di PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//Aggiungi filtro pivot
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

//Aggiungi PivotFormatCondition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

//fai i tuoi affari

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Aggiungi filtro pivot
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'Aggiungi PivotFormatCondition
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
