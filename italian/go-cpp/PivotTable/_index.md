---
title: "PivotTable Class"
linktitle: "PivotTable"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "PivotTable class. Incapsula l'oggetto che rappresenta pivottable in Go."
type: docs
weight: 200
url: /it/go-cpp/pivottable/
---

## PivotTable class

Descrizione sommaria per PivotTable.

```go

type PivotTable struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [Dispose](./dispose/) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino delle risorse non gestite. |
| [GetPivotCache](./getpivotcache/) | Ottiene la sorgente dati. |
| [IsExcel2003Compatible](./isexcel2003compatible/) | Specifica se la PivotTable è compatibile con Excel2003 durante l'aggiornamento della PivotTable,se vero, una stringa deve essere minore o uguale a 255 caratteri, quindi se la stringa è maggiore di 255 caratteri, verrà troncata. se falso, una stringa non avrà la restrizione sopra menzionata.Il valore predefinito è vero. |
| [SetIsExcel2003Compatible](./setisexcel2003compatible/) | Specifica se la PivotTable è compatibile con Excel2003 durante l'aggiornamento della PivotTable,se vero, una stringa deve essere minore o uguale a 255 caratteri, quindi se la stringa è maggiore di 255 caratteri, verrà troncata. se falso, una stringa non avrà la restrizione sopra menzionata.Il valore predefinito è vero. |
| [GetRefreshedByWho](./getrefreshedbywho/) | Ottiene il nome dell'ultimo utente che ha aggiornato questa PivotTable |
| [GetRefreshDate](./getrefreshdate/) | Ottiene l'ultima data e ora in cui il PivotTable è stato aggiornato. |
| [GetPivotTableStyle](./getpivottablestyle/) | Ottiene le impostazioni TableStyle di questa tabella pivot. |
| [SetPivotTableStyle](./setpivottablestyle/) | Ottiene le impostazioni TableStyle di questa tabella pivot. |
| [GetPivotTableStyleName](./getpivottablestylename/) | Ottiene o imposta il nome dello stile della tabella pivot. |
| [SetPivotTableStyleName](./setpivottablestylename/) | Ottiene o imposta il nome dello stile della tabella pivot. |
| [GetPivotTableStyleType](./getpivottablestyletype/) | Ottiene e imposta lo stile incorporato della tabella pivot. |
| [SetPivotTableStyleType](./setpivottablestyletype/) | Ottiene e imposta lo stile incorporato della tabella pivot. |
| [CopyStyle](./copystyle/) | Copia lo stile nominato da un'altra tabella pivot. |
| [ShowReportFilterPage](./showreportfilterpage/) | Mostra tutte le pagine del filtro report in base a PivotField, il PivotField deve trovarsi nei PageFields. |
| [ShowReportFilterPageByName](./showreportfilterpagebyname/) | Mostra tutte le pagine del filtro report in base al nome di PivotField, il PivotField deve trovarsi nei PageFields. |
| [ShowReportFilterPageByIndex](./showreportfilterpagebyindex/) | Mostra tutte le pagine del filtro report in base all'indice di posizione nei PageFields. |
| [RemoveField_PivotFieldType_String](./removefield_pivotfieldtype_string/) | Rimuove un campo da un'area campo specifica. |
| [RemoveField_PivotFieldType_Int](./removefield_pivotfieldtype_int/) | Rimuove un campo da una regione pivot specifica. |
| [RemoveField_PivotFieldType_PivotField](./removefield_pivotfieldtype_pivotfield/) | Rimuovi campo da un'area campo specifica. |
| [AddFieldToArea_PivotFieldType_String](./addfieldtoarea_pivotfieldtype_string/) | Aggiunge il campo all'area specifica. |
| [AddFieldToArea_PivotFieldType_Int](./addfieldtoarea_pivotfieldtype_int/) | Aggiunge il campo all'area specifica. |
| [AddFieldToArea_PivotFieldType_PivotField](./addfieldtoarea_pivotfieldtype_pivotfield/) | Aggiunge il campo all'area specifica. |
| [AddCalculatedField_String_String_Bool](./addcalculatedfield_string_string_bool/) | Aggiunge un campo calcolato al campo pivot. |
| [AddCalculatedField_String_String](./addcalculatedfield_string_string/) | Aggiunge un campo calcolato al campo pivot e lo trascina nell'area dati. |
| [GetFields](./getfields/) | Ottiene l'elenco specifico dei campi pivot per regione. |
| [GetColumnFields](./getcolumnfields/) | Restituisce un oggetto PivotFields che è attualmente mostrato come campi colonna. |
| [GetRowFields](./getrowfields/) | Restituisce un oggetto PivotFields che è attualmente mostrato come campi riga. |
| [GetPageFields](./getpagefields/) | Restituisce un oggetto PivotFields che è attualmente mostrato come campi pagina. |
| [GetDataFields](./getdatafields/) | Ottiene un oggetto PivotField che rappresenta tutti i campi dati in un PivotTable. Sola lettura. Viene inizializzato solo quando ci sono due o più campi dati nei DataPiovtFiels. Viene usato solo per aggiungere DataPivotField all'area riga/colonna del PivotTable. L'impostazione predefinita è nell'area riga. |
| [GetValuesField](./getvaluesfield/) | Ottiene un oggetto PivotField che rappresenta tutti i campi dati in un PivotTable. Sola lettura. Viene creato solo quando ci sono due o più campi dati nella regione Data. Per impostazione predefinita è nella regione riga. È possibile trascinarlo nella regione riga/colonna con il metodo PivotTable.AddFieldToArea(). |
| [GetBaseFields](./getbasefields/) | Restituisce tutti i campi pivot di base nel PivotTable. |
| [GetPivotFilters](./getpivotfilters/) | Restituisce tutti i filtri dei campi pivot nella tabella pivot. |
| [GetButtonArea](./getbuttonarea/) | Ottiene l'area che contiene il pulsante campo. |
| [GetTopRightArea](./gettoprightarea/) | Rappresenta l'area vuota in alto a destra del PivotTable (in alto a sinistra per i fogli RTL). |
| [GetFilterArea](./getfilterarea/) | Ottiene l'area della regione filtro. |
| [GetColumnRange](./getcolumnrange/) | Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area della colonna nel report PivotTable. Read-only. |
| [GetRowRange](./getrowrange/) | Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area della riga nel report PivotTable. Read-only. |
| [GetDataBodyRange](./getdatabodyrange/) | Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area dei dati nell'elenco tra la riga di intestazione e la riga di inserimento. Read-only. |
| [GetTableRange1](./gettablerange1/) | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report PivotTable, ma non include i campi di pagina. Read-only. |
| [GetTableRange2](./gettablerange2/) | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report PivotTable, include i campi di pagina. Read-only. |
| [MoveTo_Int_Int](./moveto_int_int/) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [MoveTo_Int_Int_Int](./moveto_int_int_int/) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [MoveTo_String](./moveto_string/) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [IsGridDropZones](./isgriddropzones/) | Indica se il report PivotTable visualizza il layout classico della pivot table (consente il trascinamento dei campi nella griglia). |
| [SetIsGridDropZones](./setisgriddropzones/) | Indica se il report PivotTable visualizza il layout classico della pivot table (consente il trascinamento dei campi nella griglia). |
| [GetShowColumnGrandTotals](./getshowcolumngrandtotals/) | Indica se mostrare i totali complessivi per le colonne di questa pivot table. |
| [SetShowColumnGrandTotals](./setshowcolumngrandtotals/) | Indica se mostrare i totali complessivi per le colonne di questa pivot table. |
| [GetShowRowGrandTotals](./getshowrowgrandtotals/) | Indica se mostrare i totali complessivi per le righe della pivot table. |
| [SetShowRowGrandTotals](./setshowrowgrandtotals/) | Indica se mostrare i totali complessivi per le righe della pivot table. |
| [GetDisplayNullString](./getdisplaynullstring/) | Indica se il report PivotTable visualizza una stringa personalizzata quando il valore è nullo. |
| [SetDisplayNullString](./setdisplaynullstring/) | Indica se il report PivotTable visualizza una stringa personalizzata quando il valore è nullo. |
| [GetNullString](./getnullstring/) | Ottiene la stringa visualizzata nelle celle che contengono valori nulli quando la proprietà DisplayNullString è true. Il valore predefinito è una stringa vuota. |
| [SetNullString](./setnullstring/) | Ottiene la stringa visualizzata nelle celle che contengono valori nulli quando la proprietà DisplayNullString è true. Il valore predefinito è una stringa vuota. |
| [GetDisplayErrorString](./getdisplayerrorstring/) | Indica se il report PivotTable visualizza una stringa personalizzata nelle celle che contengono errori. |
| [SetDisplayErrorString](./setdisplayerrorstring/) | Indica se il report PivotTable visualizza una stringa personalizzata nelle celle che contengono errori. |
| [GetDataFieldHeaderName](./getdatafieldheadername/) | Ottiene e imposta il nome dell'intestazione del campo dell'area dei valori nella PivotTable. |
| [SetDataFieldHeaderName](./setdatafieldheadername/) | Ottiene e imposta il nome dell'intestazione del campo dell'area dei valori nella PivotTable. |
| [GetErrorString](./geterrorstring/) | Ottiene la stringa visualizzata nelle celle che contengono errori quando la proprietà DisplayErrorString è true. Il valore predefinito è una stringa vuota. |
| [SetErrorString](./seterrorstring/) | Ottiene la stringa visualizzata nelle celle che contengono errori quando la proprietà DisplayErrorString è true. Il valore predefinito è una stringa vuota. |
| [IsAutoFormat](./isautoformat/) | Indica se il report PivotTable è formattato automaticamente. Casella di controllo \"autoformat table\" presente nelle opzioni della pivot table per Excel 2003. |
| [SetIsAutoFormat](./setisautoformat/) | Indica se il report PivotTable è formattato automaticamente. Casella di controllo \"autoformat table\" presente nelle opzioni della pivot table per Excel 2003. |
| [GetAutofitColumnWidthOnUpdate](./getautofitcolumnwidthonupdate/) | Indica se adattare automaticamente la larghezza della colonna durante l'aggiornamento. |
| [SetAutofitColumnWidthOnUpdate](./setautofitcolumnwidthonupdate/) | Indica se adattare automaticamente la larghezza della colonna durante l'aggiornamento. |
| [GetAutoFormatType](./getautoformattype/) | Ottiene e imposta il tipo di formattazione automatica della PivotTable. |
| [SetAutoFormatType](./setautoformattype/) | Ottiene e imposta il tipo di formattazione automatica della PivotTable. |
| [GetMergeLabels](./getmergelabels/) | Indica se i titoli di riga o colonna che si estendono su più celle devono essere uniti in un'unica cella. |
| [SetMergeLabels](./setmergelabels/) | Indica se i titoli di riga o colonna che si estendono su più celle devono essere uniti in un'unica cella. |
| [GetPreserveCellFormattingOnUpdate](./getpreservecellformattingonupdate/) | Indica se preservare la formattazione delle celle (PivotTableFormat) quando la pivot table viene aggiornata o ricalcolata. |
| [SetPreserveCellFormattingOnUpdate](./setpreservecellformattingonupdate/) | Indica se preservare la formattazione delle celle (PivotTableFormat) quando la pivot table viene aggiornata o ricalcolata. |
| [GetShowDrill](./getshowdrill/) | Ottiene e imposta la visualizzazione dei pulsanti espandi/collassa. |
| [SetShowDrill](./setshowdrill/) | Ottiene e imposta la visualizzazione dei pulsanti espandi/collassa. |
| [GetEnableDrilldown](./getenabledrilldown/) | Indica se il drilldown è abilitato. |
| [SetEnableDrilldown](./setenabledrilldown/) | Indica se il drilldown è abilitato. |
| [GetEnableFieldDialog](./getenablefielddialog/) | Indica se la finestra di dialogo Campo PivotTable è disponibile quando l'utente fa doppio clic sul campo della PivotTable. |
| [SetEnableFieldDialog](./setenablefielddialog/) | Indica se la finestra di dialogo Campo PivotTable è disponibile quando l'utente fa doppio clic sul campo della PivotTable. |
| [GetEnableFieldList](./getenablefieldlist/) | Indica se l'elenco dei campi per la PivotTable è disponibile nella visualizzazione di Excel. |
| [SetEnableFieldList](./setenablefieldlist/) | Indica se l'elenco dei campi per la PivotTable è disponibile nella visualizzazione di Excel. |
| [GetEnableWizard](./getenablewizard/) | Indica se la procedura guidata PivotTable è disponibile. |
| [SetEnableWizard](./setenablewizard/) | Indica se la procedura guidata PivotTable è disponibile. |
| [GetSubtotalHiddenPageItems](./getsubtotalhiddenpageitems/) | Indica se gli elementi di campo di pagina nascosti nel report PivotTable sono inclusi nei subtotali di riga e colonna, nei totali di blocco e nei totali complessivi. Il valore predefinito è False. |
| [SetSubtotalHiddenPageItems](./setsubtotalhiddenpageitems/) | Indica se gli elementi di campo di pagina nascosti nel report PivotTable sono inclusi nei subtotali di riga e colonna, nei totali di blocco e nei totali complessivi. Il valore predefinito è False. |
| [GetGrandTotalName](./getgrandtotalname/) | Restituisce l'etichetta visualizzata nell'intestazione della colonna o della riga del totale generale. Il valore predefinito è la stringa "Grand Total". |
| [SetGrandTotalName](./setgrandtotalname/) | Restituisce l'etichetta visualizzata nell'intestazione della colonna o della riga del totale generale. Il valore predefinito è la stringa "Grand Total". |
| [GetManualUpdate](./getmanualupdate/) | Indica se il report PivotTable viene ricalcolato solo su richiesta dell'utente. |
| [SetManualUpdate](./setmanualupdate/) | Indica se il report PivotTable viene ricalcolato solo su richiesta dell'utente. |
| [GetAllowMultipleFiltersPerField](./getallowmultiplefiltersperfield/) | Specifica un valore booleano che indica se i campi di una PivotTable possono avere più filtri impostati. |
| [SetAllowMultipleFiltersPerField](./setallowmultiplefiltersperfield/) | Specifica un valore booleano che indica se i campi di una PivotTable possono avere più filtri impostati. |
| [GetEnableDataValueEditing](./getenabledatavalueediting/) | Specifica un valore booleano che indica se all'utente è consentito modificare le celle nell'area dati della PivotTable. Abilita la modifica delle celle nell'area dei valori |
| [SetEnableDataValueEditing](./setenabledatavalueediting/) | Specifica un valore booleano che indica se all'utente è consentito modificare le celle nell'area dati della PivotTable. Abilita la modifica delle celle nell'area dei valori |
| [GetShowDataTips](./getshowdatatips/) | Indica se i tooltip devono essere visualizzati per le celle dei dati della PivotTable. |
| [SetShowDataTips](./setshowdatatips/) | Indica se i tooltip devono essere visualizzati per le celle dei dati della PivotTable. |
| [GetShowMemberPropertyTips](./getshowmemberpropertytips/) | Specifica un valore booleano che indica se le informazioni delle proprietà dei membri devono essere omesse dai tooltip della PivotTable. |
| [SetShowMemberPropertyTips](./setshowmemberpropertytips/) | Specifica un valore booleano che indica se le informazioni delle proprietà dei membri devono essere omesse dai tooltip della PivotTable. |
| [GetShowValuesRow](./getshowvaluesrow/) | Indica se mostrare la riga dei valori. |
| [SetShowValuesRow](./setshowvaluesrow/) | Indica se mostrare la riga dei valori. |
| [GetShowEmptyCol](./getshowemptycol/) | Indica se includere colonne vuote nella tabella |
| [SetShowEmptyCol](./setshowemptycol/) | Indica se includere colonne vuote nella tabella |
| [GetShowEmptyRow](./getshowemptyrow/) | Indica se includere righe vuote nella tabella. |
| [SetShowEmptyRow](./setshowemptyrow/) | Indica se includere righe vuote nella tabella. |
| [GetFieldListSortAscending](./getfieldlistsortascending/) | Indica se i campi nella PivotTable sono ordinati in un ordine non predefinito nell'elenco dei campi. |
| [SetFieldListSortAscending](./setfieldlistsortascending/) | Indica se i campi nella PivotTable sono ordinati in un ordine non predefinito nell'elenco dei campi. |
| [GetPrintDrill](./getprintdrill/) | Specifica un valore booleano che indica se gli indicatori di drill devono essere stampati. Stampa i pulsanti di espansione/contrazione quando visualizzati nella PivotTable |
| [SetPrintDrill](./setprintdrill/) | Specifica un valore booleano che indica se gli indicatori di drill devono essere stampati. Stampa i pulsanti di espansione/contrazione quando visualizzati nella PivotTable |
| [GetAltTextTitle](./getalttexttitle/) | Ottiene e imposta il titolo del testo alternativo. |
| [SetAltTextTitle](./setalttexttitle/) | Ottiene e imposta il titolo del testo alternativo. |
| [GetAltTextDescription](./getalttextdescription/) | Ottiene la descrizione del testo alternativo. |
| [SetAltTextDescription](./setalttextdescription/) | Ottiene la descrizione del testo alternativo. |
| [GetName](./getname/) | Ottiene il nome della PivotTable |
| [SetName](./setname/) | Ottiene il nome della PivotTable |
| [GetColumnHeaderCaption](./getcolumnheadercaption/) | Ottiene e imposta la didascalia personalizzata dell'intestazione di colonna della PivotTable. |
| [SetColumnHeaderCaption](./setcolumnheadercaption/) | Ottiene e imposta la didascalia personalizzata dell'intestazione di colonna della PivotTable. |
| [GetIndent](./getindent/) | Specifica l'incremento di rientro per l'asse compatto e può essere usato per impostare il layout del report in forma compatta. |
| [SetIndent](./setindent/) | Specifica l'incremento di rientro per l'asse compatto e può essere usato per impostare il layout del report in forma compatta. |
| [GetRowHeaderCaption](./getrowheadercaption/) | Ottiene e imposta la didascalia personalizzata dell'intestazione di riga in questa PivotTable. |
| [SetRowHeaderCaption](./setrowheadercaption/) | Ottiene e imposta la didascalia personalizzata dell'intestazione di riga in questa PivotTable. |
| [GetShowHeaders](./getshowheaders/) | Indica se mostrare le didascalie dei campi dati e le didascalie dei campi pivot sull'asse delle righe e sull'asse delle colonne nella visualizzazione della PivotTable. |
| [SetShowHeaders](./setshowheaders/) | Indica se mostrare le didascalie dei campi dati e le didascalie dei campi pivot sull'asse delle righe e sull'asse delle colonne nella visualizzazione della PivotTable. |
| [GetCustomListSort](./getcustomlistsort/) | Indica se considerare l'elenco personalizzato incorporato durante l'ordinamento dei dati |
| [SetCustomListSort](./setcustomlistsort/) | Indica se considerare l'elenco personalizzato incorporato durante l'ordinamento dei dati |
| [GetConditionalFormats](./getconditionalformats/) | Ottiene i formati condizionali della PivotTable. |
| [GetPageFieldOrder](./getpagefieldorder/) | Ottiene e imposta l'ordine in cui i campi pagina vengono aggiunti al layout del report della PivotTable. |
| [SetPageFieldOrder](./setpagefieldorder/) | Ottiene e imposta l'ordine in cui i campi pagina vengono aggiunti al layout del report della PivotTable. |
| [GetPageFieldWrapCount](./getpagefieldwrapcount/) | Ottiene il numero di campi pagina in ogni colonna o riga nel report della PivotTable. |
| [SetPageFieldWrapCount](./setpagefieldwrapcount/) | Ottiene il numero di campi pagina in ogni colonna o riga nel report della PivotTable. |
| [GetTag](./gettag/) | Ottiene e imposta una stringa definita dall'utente associata a questa visualizzazione della PivotTable. |
| [SetTag](./settag/) | Ottiene e imposta una stringa definita dall'utente associata a questa visualizzazione della PivotTable. |
| [GetSaveData](./getsavedata/) | Indica se i dati del report PivotTable vengono salvati con la cartella di lavoro. |
| [SetSaveData](./setsavedata/) | Indica se i dati del report PivotTable vengono salvati con la cartella di lavoro. |
| [GetRefreshDataOnOpeningFile](./getrefreshdataonopeningfile/) | Indica se aggiornare i dati all'apertura del file. |
| [SetRefreshDataOnOpeningFile](./setrefreshdataonopeningfile/) | Indica se aggiornare i dati all'apertura del file. |
| [GetSourceType](./getsourcetype/) | Ottiene il tipo di origine dati della tabella pivot. |
| [GetSourceDataConnections](./getsourcedataconnections/) | Ottiene le origini dati della connessione esterna. |
| [GetNamesOfSourceDataConnections](./getnamesofsourcedataconnections/) | Ottiene i nomi delle connessioni dati di origine esterna. |
| [GetDataSource](./getdatasource/) | Ottiene e imposta l'origine dati della tabella pivot. |
| [SetDataSource](./setdatasource/) | Ottiene e imposta l'origine dati della tabella pivot. |
| [ChangeDataSource](./changedatasource/) | Modifica l'origine dati della tabella pivot. |
| [GetSource](./getsource/) | Ottieni l'origine dati di questa tabella pivot. |
| [GetSource_Bool](./getsource_bool/) | Ottieni l'origine dati di questa tabella pivot. |
| [Refresh](./refresh/) | Aggiorna il PivotCache dall'origine dati e calcola i dati e lo stile per la visualizzazione pivot. |
| [CalculateData](./calculatedata/) | Calcola i dati della tabella pivot nelle celle. |
| [CalculateData_PivotTableCalculateOption](./calculatedata_pivottablecalculateoption/) | Calcola la tabella pivot con opzioni. |
| [GetPivotTablesWithSamePivotCache](./getpivottableswithsamepivotcache/) | Ottiene tutte le tabelle pivot con la stessa cache pivot. |
| [ClearData](./cleardata/) | Cancella i dati e la formattazione della visualizzazione della tabella pivot. |
| [ClearFilters](./clearfilters/) | Cancella tutti i filtri di questa tabella pivot. |
| [ClearAll](./clearall/) | Rimuove tutti i campi dalle regioni. |
| [CalculateRange](./calculaterange/) | Calcola l'intervallo della tabella pivot. |
| [FormatAll](./formatall/) | Formatta tutte le celle nell'area della tabella pivot |
| [FormatRow](./formatrow/) | Formatta i dati della riga nell'area della tabella pivot |
| [Format_PivotArea_Style](./format_pivotarea_style/) | Formatta l'area selezionata della tabella pivot. |
| [Format_CellArea_Style](./format_cellarea_style/) | Formatta l'area selezionata della tabella pivot. |
| [Format_Int_Int_Style](./format_int_int_style/) | Formatta la cella nell'area della tabella pivot |
| [SelectArea](./selectarea/) | Seleziona un'area della visualizzazione della tabella pivot. |
| [ShowDetail](./showdetail/) | Mostra il dettaglio di un elemento nella regione dati in una nuova tabella. |
| [GetPivotFormats](./getpivotformats/) | Ottiene tutti i formati applicati alla tabella pivot. |
| [GetRepeatItemsOnEachPrintedPage](./getrepeatitemsoneachprintedpage/) | Indica se le didascalie dell'elemento pivot nell'area delle righe sono ripetute su ogni pagina stampata per i campi pivot in forma tabellare. |
| [SetRepeatItemsOnEachPrintedPage](./setrepeatitemsoneachprintedpage/) | Indica se le didascalie dell'elemento pivot nell'area delle righe sono ripetute su ogni pagina stampata per i campi pivot in forma tabellare. |
| [GetPrintTitles](./getprinttitles/) | Indica se i titoli di stampa per il foglio di lavoro sono impostati in base al report della tabella pivot. Il valore predefinito è false. |
| [SetPrintTitles](./setprinttitles/) | Indica se i titoli di stampa per il foglio di lavoro sono impostati in base al report della tabella pivot. Il valore predefinito è false. |
| [GetDisplayImmediateItems](./getdisplayimmediateitems/) | Indica se gli elementi nelle aree di riga e colonna sono visibili quando l'area dati della tabella pivot è vuota. Il valore predefinito è true. |
| [SetDisplayImmediateItems](./setdisplayimmediateitems/) | Indica se gli elementi nelle aree di riga e colonna sono visibili quando l'area dati della tabella pivot è vuota. Il valore predefinito è true. |
| [IsSelected](./isselected/) | Indica se questa tabella pivot è selezionata. |
| [SetIsSelected](./setisselected/) | Indica se questa tabella pivot è selezionata. |
| [GetShowPivotStyleRowHeader](./getshowpivotstylerowheader/) | Indica se l'intestazione di riga nella tabella pivot deve avere lo stile applicato. |
| [SetShowPivotStyleRowHeader](./setshowpivotstylerowheader/) | Indica se l'intestazione di riga nella tabella pivot deve avere lo stile applicato. |
| [GetShowPivotStyleColumnHeader](./getshowpivotstylecolumnheader/) | Indica se l'intestazione di colonna nella tabella pivot deve avere lo stile applicato. |
| [SetShowPivotStyleColumnHeader](./setshowpivotstylecolumnheader/) | Indica se l'intestazione di colonna nella tabella pivot deve avere lo stile applicato. |
| [GetShowPivotStyleRowStripes](./getshowpivotstylerowstripes/) | Indica se la formattazione a righe alternate è applicata. |
| [SetShowPivotStyleRowStripes](./setshowpivotstylerowstripes/) | Indica se la formattazione a righe alternate è applicata. |
| [GetShowPivotStyleColumnStripes](./getshowpivotstylecolumnstripes/) | Indica se la formattazione a strisce è applicata per la colonna. |
| [SetShowPivotStyleColumnStripes](./setshowpivotstylecolumnstripes/) | Indica se la formattazione a strisce è applicata per la colonna. |
| [GetShowPivotStyleLastColumn](./getshowpivotstylelastcolumn/) | Indica se la formattazione della colonna è applicata. |
| [SetShowPivotStyleLastColumn](./setshowpivotstylelastcolumn/) | Indica se la formattazione della colonna è applicata. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Ottiene le interruzioni di pagina orizzontali di questa tabella pivot. |
| [ShowInCompactForm](./showincompactform/) | Disposizione della vista della tabella pivot in forma compatta. |
| [ShowInOutlineForm](./showinoutlineform/) | Disposizione della tabella pivot in forma outline. |
| [ShowInTabularForm](./showintabularform/) | Disposizione della tabella pivot in forma tabellare. |
| [GetCellByDisplayName](./getcellbydisplayname/) | Ottiene l'oggetto Cell in base al nome visualizzato di PivotField. |
| [GetDependentPivotTables](./getdependentpivottables/) | Ottiene tutte le tabelle Pivot che utilizzano questa tabella Pivot come origine dati. |
| [ExportViewToJson](./exportviewtojson/) | Esporta la vista pivot come JSON. |
