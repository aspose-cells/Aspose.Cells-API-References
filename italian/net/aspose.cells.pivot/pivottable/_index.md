---
title: "Classe PivotTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotTable. Descrizione sommaria per PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Descrizione riepilogativa per la PivotTable.

```csharp
public class PivotTable : IDisposable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllowMultipleFiltersPerField](../../aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/) { get; set; } | Specifica un valore booleano che indica se i campi di una PivotTable possono avere più filtri impostati su di essi. |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription/) { get; set; } | Ottiene la descrizione del testo alternativo. |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle/) { get; set; } | Ottiene e imposta il titolo del testo alternativo. |
| [AutofitColumnWidthOnUpdate](../../aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/) { get; set; } | Indica se adattare automaticamente la larghezza della colonna all'aggiornamento |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype/) { get; set; } | Ottiene e imposta il tipo di formattazione automatica della PivotTable. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields/) { get; } | Restituisce tutti i campi pivot di base nella PivotTable. |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields/) { get; } | Restituisce un oggetto PivotFields che è attualmente mostrato come campi colonna. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand/) { get; set; } | (**Obsolete.**) Indica se il report PivotTable mostra i totali generali per le colonne. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption/) { get; set; } | Ottiene e imposta la didascalia personalizzata dell'intestazione di colonna della PivotTable. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange/) { get; } | Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area colonna nel report PivotTable. Sola lettura. |
| [ConditionalFormats](../../aspose.cells.pivot/pivottable/conditionalformats/) { get; } | Ottiene i formati condizionali della pivot table. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort/) { get; set; } | Indica se considerare l'elenco personalizzato integrato durante l'ordinamento dei dati |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange/) { get; } | Restituisce un oggetto [`CellArea`](../../aspose.cells/cellarea/) che rappresenta l'intervallo che contiene l'area dati nell'elenco tra la riga di intestazione e la riga di inserimento. Sola lettura. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield/) { get; } | (**Obsolete.**) Ottiene un oggetto [`PivotField`](../pivotfield/) che rappresenta tutti i campi dati in una PivotTable. Sola lettura. Viene creato solo quando ci sono due o più campi dati nella regione Dati. Per impostazione predefinita è nella regione di riga. È possibile trascinarlo nella regione riga/colonna con il metodo PivotTable.AddFieldToArea(). |
| [DataFieldHeaderName](../../aspose.cells.pivot/pivottable/datafieldheadername/) { get; set; } | Ottiene e imposta il nome dell'intestazione del campo dell'area valori nella PivotTable. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields/) { get; } | Ottiene una [`PivotFieldCollection`](../pivotfieldcollection/) che rappresenta tutti i campi dati in una PivotTable. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource/) { get; set; } | Ottiene e imposta l'origine dati della pivot table. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring/) { get; set; } | Indica se il report PivotTable visualizza una stringa personalizzata nelle celle che contengono errori. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems/) { get; set; } | Indica se gli elementi nelle aree riga e colonna sono visibili quando l'area dati della PivotTable è vuota. Il valore predefinito è true. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring/) { get; set; } | Indica se il report PivotTable visualizza una stringa personalizzata se il valore è null. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting/) { get; set; } | Specifica un valore booleano che indica se all'utente è consentito modificare le celle nell'area dati della PivotTable. Il valore predefinito è false. |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown/) { get; set; } | Indica se il drilldown è abilitato. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog/) { get; set; } | Indica se la finestra di dialogo Campo PivotTable è disponibile quando l'utente fa doppio clic sul campo PivotTable. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist/) { get; set; } | Indica se l'elenco dei campi per la PivotTable è disponibile nella visualizzazione di Excel. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard/) { get; set; } | Indica se la procedura guidata PivotTable è disponibile. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring/) { get; set; } | Restituisce la stringa visualizzata nelle celle che contengono errori quando la proprietà DisplayErrorString è true. Il valore predefinito è una stringa vuota. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource/) { get; } | (**Obsolete.**) Restituisce la fonte dati della connessione esterna. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending/) { get; set; } | Indica se i campi nella PivotTable sono ordinati in un ordine non predefinito nell'elenco dei campi. |
| [FilterArea](../../aspose.cells.pivot/pivottable/filterarea/) { get; } | Restituisce l'area della regione filtro. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname/) { get; set; } | Restituisce l'etichetta visualizzata nell'intestazione della colonna o della riga del totale generale. Il valore predefinito è la stringa "Grand Total". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows/) { get; set; } | (**Obsolete.**) Indica se aggiungere righe vuote. Questa proprietà si applica solo ai tipi di autoformattazione PivotTable che richiedono l'aggiunta di righe vuote. |
| [Indent](../../aspose.cells.pivot/pivottable/indent/) { get; set; } | Specifica l'incremento di rientro per l'asse compatto e può essere usato per impostare il Layout del report in Forma compatta. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat/) { get; set; } | Indica se il report PivotTable è formattato automaticamente. Casella di controllo "autoformat table" presente nelle opzioni PivotTable per Excel 2003. |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible/) { get; set; } | Specifica se la PivotTable è compatibile con Excel2003 durante l'aggiornamento della PivotTable; se true, una stringa deve essere lunga al massimo 255 caratteri, quindi se la stringa supera i 255 caratteri verrà troncata. Se false, una stringa non avrà la suddetta restrizione. Il valore predefinito è true. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones/) { get; set; } | Indica se il report PivotTable visualizza il layout classico della PivotTable. (consente il trascinamento dei campi nella griglia) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters/) { get; set; } | (**Obsolete.**) Specifica un valore booleano che indica se i campi di una PivotTable possono avere più filtri impostati. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected/) { get; set; } | Indica se questa PivotTable è selezionata. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles/) { get; set; } | (**Obsolete.**) Indica se i nomi di PivotItem devono essere ripetuti nella parte superiore di ogni pagina stampata. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate/) { get; set; } | Indica se il report PivotTable viene ricalcolato solo su richiesta dell'utente. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels/) { get; set; } | Restituisce o imposta se unire le etichette dei campi riga/colonna che si estendono su più celle. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit/) { get; set; } | (**Obsolete.**) Specifica un valore booleano che indica se i campi di una PivotTable possono avere più filtri impostati. |
| [Name](../../aspose.cells.pivot/pivottable/name/) { get; set; } | Restituisce il nome della PivotTable |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring/) { get; set; } | Restituisce la stringa visualizzata nelle celle che contengono valori null quando la proprietà DisplayNullString è true. Il valore predefinito è una stringa vuota. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder/) { get; set; } | Restituisce e imposta l'ordine in cui i campi pagina vengono aggiunti al layout del report PivotTable. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields/) { get; } | Restituisce una [`PivotFieldCollection`](../pivotfieldcollection/) attualmente mostrata come campi pagina. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount/) { get; set; } | Restituisce il numero di campi pagina in ciascuna colonna o riga del report PivotTable. |
| [PivotCache](../../aspose.cells.pivot/pivottable/pivotcache/) { get; } | Restituisce la fonte dati. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters/) { get; } | Restituisce tutti i filtri nella tabella pivot. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions/) { get; } | (**Obsolete.**) Ottiene le condizioni di formato della tabella pivot. |
| [PivotFormats](../../aspose.cells.pivot/pivottable/pivotformats/) { get; } | Ottiene tutti i formati di cella applicati a questa tabella pivot. |
| [PivotTableStyle](../../aspose.cells.pivot/pivottable/pivottablestyle/) { get; set; } | Ottiene le impostazioni di TableStyle di questa tabella pivot. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename/) { get; set; } | Ottiene o imposta il nome dello stile della tabella pivot. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype/) { get; set; } | Ottiene e imposta lo stile predefinito della tabella pivot. |
| [PreserveCellFormattingOnUpdate](../../aspose.cells.pivot/pivottable/preservecellformattingonupdate/) { get; set; } | Indica se conservare la formattazione delle celle ([`PivotTableFormat`](../pivottableformat/)) quando la tabella pivot viene aggiornata o ricalcolata. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting/) { get; set; } | (**Obsolete.**) Indica se la formattazione delle celle ([`PivotTableFormat`](../pivottableformat/)) è conservata quando la PivotTable viene aggiornata o ricalcolata. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill/) { get; set; } | Specifica un valore booleano che indica se gli indicatori di drill devono essere stampati. Stampa i pulsanti di espansione/collasso quando visualizzati nella tabella pivot. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles/) { get; set; } | Indica se i titoli di stampa per il foglio di lavoro sono impostati in base al report della PivotTable. Il valore predefinito è false. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile/) { get; set; } | Indica se aggiornare i dati all'apertura del file. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate/) { get; } | Ottiene la data e l'ora dell'ultimo aggiornamento della PivotTable. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho/) { get; } | Ottiene il nome dell'ultimo utente che ha aggiornato questa PivotTable |
| [RepeatItemsOnEachPrintedPage](../../aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/) { get; set; } | Indica se le didascalie degli elementi pivot nell'area righe sono ripetute su ogni pagina stampata per i campi pivot in forma tabellare. |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields/) { get; } | Restituisce una [`PivotFieldCollection`](../pivotfieldcollection/) attualmente mostrata come campi di riga. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand/) { get; set; } | (**Obsolete.**) Indica se mostrare i totali complessivi per le righe di questa tabella pivot. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption/) { get; set; } | Ottiene e imposta la didascalia personalizzata dell'intestazione di riga in questa PivotTable. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange/) { get; } | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'area di riga nel report della PivotTable. Sola lettura. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata/) { get; set; } | Indica se i dati del report della PivotTable sono salvati con la cartella di lavoro. |
| [ShowColumnGrandTotals](../../aspose.cells.pivot/pivottable/showcolumngrandtotals/) { get; set; } | Indica se mostrare i totali complessivi per le colonne di questa tabella pivot. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips/) { get; set; } | Indica se i suggerimenti devono essere visualizzati per le celle dati della PivotTable. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill/) { get; set; } | Ottiene e imposta se mostrare i pulsanti di espansione/collasso. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol/) { get; set; } | Indica se includere colonne vuote nella tabella |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow/) { get; set; } | Indica se includere righe vuote nella tabella. |
| [ShowHeaders](../../aspose.cells.pivot/pivottable/showheaders/) { get; set; } | Indica se mostrare le didascalie dei campi dati e le didascalie dei campi pivot sull'asse delle righe e sull'asse delle colonne nella visualizzazione della PivotTable. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips/) { get; set; } | Specifica un valore booleano che indica se le informazioni delle proprietà dei membri devono essere omesse dai suggerimenti della PivotTable. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader/) { get; set; } | Indica se l'intestazione della colonna nella tabella pivot deve avere lo stile applicato. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/) { get; set; } | Indica se la formattazione a strisce è applicata per la colonna. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn/) { get; set; } | Indica se la formattazione della colonna è applicata. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader/) { get; set; } | Indica se l'intestazione della riga nella tabella pivot deve avere lo stile applicato. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes/) { get; set; } | Indica se la formattazione a strisce per le righe è applicata. |
| [ShowRowGrandTotals](../../aspose.cells.pivot/pivottable/showrowgrandtotals/) { get; set; } | Indica se mostrare i totali complessivi per le righe della tabella pivot. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption/) { get; set; } | (**Obsolete.**) Indica se la didascalia dell'intestazione della riga è mostrata nel report PivotTable Indica se visualizzare le didascalie dei campi e i menu a discesa dei filtri |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow/) { get; set; } | Indica se mostrare la riga dei valori. |
| [SourceType](../../aspose.cells.pivot/pivottable/sourcetype/) { get; } | Ottiene il tipo di origine dati della tabella pivot. |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems/) { get; set; } | Indica se gli elementi dei campi pagina nascosti nel report PivotTable sono inclusi nei subtotali di riga e colonna, nei totali di blocco e nei totali complessivi. Il valore predefinito è False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1/) { get; } | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report PivotTable, ma non include i campi pagina. Sola lettura. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2/) { get; } | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report PivotTable, includendo i campi pagina. Sola lettura. |
| [Tag](../../aspose.cells.pivot/pivottable/tag/) { get; set; } | Ottiene e imposta una stringa definita dall'utente associata a questa visualizzazione della PivotTable. |
| [TopRightArea](../../aspose.cells.pivot/pivottable/toprightarea/) { get; } | Rappresenta l'area vuota in alto a destra della PivotTable (in alto a sinistra per i fogli RTL). |
| [ValuesField](../../aspose.cells.pivot/pivottable/valuesfield/) { get; } | Ottiene un oggetto [`PivotField`](../pivotfield/) che rappresenta tutti i campi dati in una PivotTable. Sola lettura. Viene creato solo quando ci sono due o più campi dati nella regione Dati. Per impostazione predefinita si trova nella regione delle righe. È possibile trascinarlo nella regione riga/colonna con il metodo PivotTable.AddFieldToArea(). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield)(string, string) | Aggiunge un campo calcolato al campo pivot e lo trascina nell'area dati. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield_1)(string, string, bool) | Aggiunge un campo calcolato al campo pivot. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_1)(PivotFieldType, int) | Aggiunge il campo all'area specifica. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea)(PivotFieldType, PivotField) | Aggiunge il campo all'area specifica. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_2)(PivotFieldType, string) | Aggiunge il campo all'area specifica. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata_1)() | Calcola i dati della PivotTable nelle celle. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata)(PivotTableCalculateOption) | Calcola la tabella pivot con opzioni. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange/)() | Calcola l'intervallo della PivotTable. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource/)(string[]) | Modifica l'origine dati della tabella pivot. |
| [ClearAll](../../aspose.cells.pivot/pivottable/clearall/)() | Rimuove tutti i campi dalle regioni. |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata/)() | Cancella i dati e la formattazione della visualizzazione della PivotTable. |
| [ClearFilters](../../aspose.cells.pivot/pivottable/clearfilters/)() | Cancella tutti i filtri di questa tabella pivot. |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle/)(PivotTable) | Copia lo stile denominato da un'altra tabella pivot. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose/)() | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [ExportViewToJson](../../aspose.cells.pivot/pivottable/exportviewtojson/)(PivotViewToJsonOptions) | Esporta la vista pivot come JSON. |
| [Fields](../../aspose.cells.pivot/pivottable/fields/)(PivotFieldType) | (**Obsolete.**) Ottiene i campi specifici per tipo di campo. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format)(CellArea, Style) | Formatta l'area selezionata della PivotTable. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_1)(PivotArea, Style) | Formatta l'area selezionata della PivotTable. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_2)(int, int, Style) | Formatta la cella nell'area della pivottable. |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall/)(Style) | Formatta tutte le celle nell'area della pivottable. |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow/)(int, Style) | Formatta i dati della riga nell'area della pivottable. |
| [GetButtonArea](../../aspose.cells.pivot/pivottable/getbuttonarea/)(PivotFieldType) | Ottiene l'area che contiene il pulsante del campo. |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname/)(string) | Ottiene l'oggetto [`Cell`](../../aspose.cells/cell/) per nome visualizzato di PivotField. |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren/)() | (**Obsolete.**) Ottiene le Pivot Table figlie che utilizzano i dati di questa PivotTable come origine dati. |
| [GetDependentPivotTables](../../aspose.cells.pivot/pivottable/getdependentpivottables/)() | Ottiene tutte le `PivotTable` che usano questa PivotTable come origine dati. |
| [GetFields](../../aspose.cells.pivot/pivottable/getfields/)(PivotFieldType) | Ottiene l'elenco specifico dei campi pivot per regione. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks/)() | (**Obsolete.**) Ottiene l'elenco degli indici di riga della tabella pivot per interruzioni di pagina orizzontali |
| [GetHorizontalPageBreaks](../../aspose.cells.pivot/pivottable/gethorizontalpagebreaks/)() | Ottiene le interruzioni di pagina orizzontali di questa tabella pivot. |
| [GetNamesOfSourceDataConnections](../../aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/)() | Ottiene i nomi delle connessioni dati di origine esterna. |
| [GetPivotTablesWithSamePivotCache](../../aspose.cells.pivot/pivottable/getpivottableswithsamepivotcache/)() | Ottiene tutte le tabelle pivot con la stessa cache pivot. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource)() | Ottieni l'origine dati di questa tabella pivot. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource_1)(bool) | Ottieni l'origine dati di questa tabella pivot. |
| [GetSourceDataConnections](../../aspose.cells.pivot/pivottable/getsourcedataconnections/)() | Ottiene le origini dati delle connessioni esterne. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move_1)(string) | (**Obsolete.**) Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move)(int, int) | (**Obsolete.**) Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [MoveItem](../../aspose.cells.pivot/pivottable/moveitem/)(PivotFieldType, string[], bool, int) | Sposta un elemento su o giù. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_2)(string) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto)(int, int) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_1)(int, int, int) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh)() | Aggiorna [`PivotCache`](./pivotcache/) dall'origine dati e calcola dati e stile per la vista pivot. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh_1)(PivotTableRefreshOption) | Aggiorna [`PivotCache`](./pivotcache/) dall'origine dati e calcola dati e stile per la vista pivot. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata)() | (**Obsolete.**) Aggiorna i dati dalla sua origine dati alla cache pivot. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata_1)(PivotTableRefreshOption) | (**Obsolete.**) Aggiorna i dati e le impostazioni della pivottable dalla sua origine dati con opzioni. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_1)(PivotFieldType, int) | Rimuove un campo da una specifica regione pivot. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield)(PivotFieldType, PivotField) | Rimuovi il campo da una specifica area di campo |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_2)(PivotFieldType, string) | Rimuove un campo da un'area di campo specifica |
| [SelectArea](../../aspose.cells.pivot/pivottable/selectarea/)(CellArea) | Seleziona un'area della visualizzazione della tabella pivot. |
| [ShowDetail](../../aspose.cells.pivot/pivottable/showdetail/)(int, int, bool, int, int) | Mostra il dettaglio di un elemento nella regione dati in una nuova tabella. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform/)() | Disposizione della visualizzazione della tabella pivot in forma compatta. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform/)() | Disposizione della tabella pivot in forma outline. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform/)() | Disposizione della tabella pivot in forma tabellare. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage/)(PivotField) | Mostra tutte le pagine di filtro del report in base a PivotField, il PivotField deve trovarsi nei PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex/)(int) | Mostra tutte le pagine di filtro del report in base all'indice di posizione nei PageFields. |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname/)(string) | Mostra tutte le pagine di filtro del report in base al nome di PivotField, il PivotField deve trovarsi nei PageFields. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotTableDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Imposta dati di esempio
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Crea tabella pivot
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];

            // Aggiungi campi
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Stilizza la tabella pivot
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Personalizza il campo di riga
            PivotField rowField = pivot.RowFields[0];
            rowField.DisplayName = "Fruit Category";

            // Aggiorna e calcola i dati
            pivot.RefreshData();
            pivot.CalculateData();

            // Salva la cartella di lavoro
            book.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


