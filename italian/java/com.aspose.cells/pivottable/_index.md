---
title: "Tabella pivot"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Descrizione riepilogativa per PivotTable."
type: docs
url: /it/java/com.aspose.cells/pivottable/
---

**Inheritance:**
java.lang.Object
```
public class PivotTable
```

Descrizione riepilogativa per PivotTable.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
          PivotTableCalculateOption calculateOption = new PivotTableCalculateOption();
          calculateOption.setRefreshData(true);
          calculateOption.setRefreshCharts(true);
          pivot.calculateData(calculateOption); 
 
         //do your business
 
         book.save("out.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addCalculatedField(String name, String formula)](#addCalculatedField-java.lang.String-java.lang.String-) | Aggiunge un campo calcolato al campo pivot e lo trascina nell'area dati. |
| [addCalculatedField(String name, String formula, boolean dragToDataArea)](#addCalculatedField-java.lang.String-java.lang.String-boolean-) | Aggiunge un campo calcolato al campo pivot. |
| [addFieldToArea(int fieldType, PivotField pivotField)](#addFieldToArea-int-com.aspose.cells.PivotField-) | Aggiunge il campo all'area specifica. |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Aggiunge il campo all'area specifica. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Aggiunge il campo all'area specifica. |
| [calculateData()](#calculateData--) | Calcola i dati della tabella pivot nelle celle. |
| [calculateData(PivotTableCalculateOption option)](#calculateData-com.aspose.cells.PivotTableCalculateOption-) | Calcola la tabella pivot con opzioni. |
| [calculateRange()](#calculateRange--) | Calcola l'intervallo della tabella pivot. |
| [changeDataSource(String[] source)](#changeDataSource-java.lang.String---) | Modifica l'origine dati della tabella pivot. |
| [clearAll()](#clearAll--) | Rimuove tutti i campi dalle regioni. |
| [clearData()](#clearData--) | Cancella i dati e la formattazione della vista della tabella pivot. |
| [clearFilters()](#clearFilters--) | Cancella tutti i filtri di questa tabella pivot. |
| [copyStyle(PivotTable pivotTable)](#copyStyle-com.aspose.cells.PivotTable-) | Copia lo stile denominato da un'altra tabella pivot. |
| [dispose()](#dispose--) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportViewToJson(PivotViewToJsonOptions options)](#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-) | Esporta la vista pivot come JSON. |
| [fields(int fieldType)](#fields-int-) | Ottiene i campi specifici per tipo di campo. |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | Formatta l'area selezionata della Tabella Pivot. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | Formatta l'area selezionata della Tabella Pivot. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | Formatta la cella nell'area della tabella pivot |
| [formatAll(Style style)](#formatAll-com.aspose.cells.Style-) | Formatta tutte le celle nell'area della tabella pivot |
| [formatRow(int row, Style style)](#formatRow-int-com.aspose.cells.Style-) | Formatta i dati della riga nell'area della tabella pivot |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--) | Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati. |
| [getAltTextDescription()](#getAltTextDescription--) | Ottiene la descrizione del testo alternativo. |
| [getAltTextTitle()](#getAltTextTitle--) | Ottiene il titolo del testo alternativo. |
| [getAutoFormatType()](#getAutoFormatType--) | Ottiene il tipo di formato automatico della Tabella Pivot. |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--) | Indica se adattare automaticamente la larghezza della colonna all'aggiornamento |
| [getBaseFields()](#getBaseFields--) | Restituisce tutti i campi pivot di base nella Tabella Pivot. |
| [getButtonArea(int axisType)](#getButtonArea-int-) | Ottiene l'area che contiene il pulsante del campo. |
| [getCellByDisplayName(String displayName)](#getCellByDisplayName-java.lang.String-) | Ottiene l'oggetto [Cell](../../com.aspose.cells/cell) per il nome visualizzato del PivotField. |
| [getChildren()](#getChildren--) | Ottiene le tabelle pivot figlie che utilizzano questi dati della Tabella Pivot come origine dati. |
| [getClass()](#getClass--) |  |
| [getColumnFields()](#getColumnFields--) | Restituisce un oggetto PivotFields che è attualmente mostrato come campi di colonna. |
| [getColumnGrand()](#getColumnGrand--) | Indica se il report della Tabella Pivot mostra i totali generali per le colonne. |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--) | Ottiene la didascalia personalizzata dell'intestazione di colonna della Tabella Pivot. |
| [getColumnRange()](#getColumnRange--) | Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area di colonna nel report della Tabella Pivot. |
| [getConditionalFormats()](#getConditionalFormats--) | Ottiene i formati condizionali della tabella pivot. |
| [getCustomListSort()](#getCustomListSort--) | Indica se considerare l'elenco personalizzato integrato durante l'ordinamento dei dati |
| [getDataBodyRange()](#getDataBodyRange--) | Restituisce un oggetto [CellArea](../../com.aspose.cells/cellarea) che rappresenta l'intervallo che contiene l'area dati nell'elenco tra la riga di intestazione e la riga di inserimento. |
| [getDataField()](#getDataField--) | Ottiene un oggetto [PivotField](../../com.aspose.cells/pivotfield) che rappresenta tutti i campi dati in una Tabella Pivot. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--) | Restituisce il nome dell'intestazione del campo dell'area valori nella PivotTable. |
| [getDataFields()](#getDataFields--) | Restituisce una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) che rappresenta tutti i campi dati in una PivotTable. |
| [getDataSource()](#getDataSource--) | Restituisce l'origine dati della PivotTable. |
| [getDependentPivotTables()](#getDependentPivotTables--) | Restituisce tutte le [PivotTable](../../com.aspose.cells/pivottable) che utilizzano questa PivotTable come origine dati. |
| [getDisplayErrorString()](#getDisplayErrorString--) | Indica se il report della PivotTable visualizza una stringa personalizzata nelle celle che contengono errori. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--) | Indica se gli elementi nelle aree riga e colonna sono visibili quando l'area dati della PivotTable è vuota. |
| [getDisplayNullString()](#getDisplayNullString--) | Indica se il report della PivotTable visualizza una stringa personalizzata se il valore è nullo. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--) | Specifica un valore booleano che indica se all'utente è consentito modificare le celle nell'area dati della PivotTable. |
| [getEnableDrilldown()](#getEnableDrilldown--) | Indica se il drilldown è abilitato. |
| [getEnableFieldDialog()](#getEnableFieldDialog--) | Indica se la finestra di dialogo PivotTable Field è disponibile quando l'utente fa doppio clic sul campo della PivotTable. |
| [getEnableFieldList()](#getEnableFieldList--) | Indica se l'elenco dei campi per la PivotTable è disponibile nella visualizzazione di Excel. |
| [getEnableWizard()](#getEnableWizard--) | Indica se la procedura guidata PivotTable è disponibile. |
| [getErrorString()](#getErrorString--) | Restituisce la stringa visualizzata nelle celle che contengono errori quando la proprietà DisplayErrorString è true. Il valore predefinito è una stringa vuota. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--) | Restituisce l'origine dati della connessione esterna. |
| [getFieldListSortAscending()](#getFieldListSortAscending--) | Indica se i campi nella PivotTable sono ordinati in un ordine non predefinito nell'elenco dei campi. |
| [getFields(int fieldType)](#getFields-int-) | Restituisce l'elenco specifico dei campi pivot per regione. |
| [getFilterArea()](#getFilterArea--) | Restituisce l'area della regione filtro. |
| [getGrandTotalName()](#getGrandTotalName--) | Restituisce l'etichetta visualizzata nell'intestazione della colonna o della riga del totale generale. |
| [getHorizontalBreaks()](#getHorizontalBreaks--) | Restituisce l'elenco degli indici di riga della tabella pivot per le interruzioni di pagina orizzontali |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Restituisce le interruzioni di pagina orizzontali di questa tabella pivot. |
| [getIndent()](#getIndent--) | Specifica l'incremento di rientro per l'asse compatto e può essere usato per impostare il Layout del report su Forma compatta. |
| [getItemPrintTitles()](#getItemPrintTitles--) | Indica se i nomi di PivotItem devono essere ripetuti nella parte superiore di ogni pagina stampata. |
| [getManualUpdate()](#getManualUpdate--) | Indica se il report della PivotTable viene ricalcolato solo su richiesta dell'utente. |
| [getMergeLabels()](#getMergeLabels--) | Restituisce se unire le etichette dei campi riga/colonna che si estendono su più celle. |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati. |
| [getName()](#getName--) | Restituisce il nome della PivotTable |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--) | Restituisce i nomi delle connessioni dati di origine esterne. |
| [getNullString()](#getNullString--) | Restituisce la stringa visualizzata nelle celle che contengono valori null quando la proprietà DisplayNullString è true. Il valore predefinito è una stringa vuota. |
| [getPageFieldOrder()](#getPageFieldOrder--) | Restituisce l'ordine in cui i campi pagina vengono aggiunti al layout del report PivotTable. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--) | Restituisce il numero di campi pagina in ogni colonna o riga del report PivotTable. |
| [getPageFields()](#getPageFields--) | Restituisce una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) che è attualmente mostrata come campi pagina. |
| [getPivotCache()](#getPivotCache--) | Restituisce l'origine dati. |
| [getPivotFilters()](#getPivotFilters--) | Restituisce tutti i filtri nella tabella pivot. |
| [getPivotFormatConditions()](#getPivotFormatConditions--) | Restituisce le Condizioni di Formato della tabella pivot. |
| [getPivotFormats()](#getPivotFormats--) | Restituisce tutti i formati cella applicati a questa tabella pivot. |
| [getPivotTableStyle()](#getPivotTableStyle--) | Restituisce le impostazioni di [TableStyle](../../com.aspose.cells/tablestyle) di questa tabella pivot. |
| [getPivotTableStyleName()](#getPivotTableStyleName--) | Restituisce il nome dello stile della tabella pivot. |
| [getPivotTableStyleType()](#getPivotTableStyleType--) | Restituisce lo stile predefinito della tabella pivot. |
| [getPivotTablesWithSamePivotCache()](#getPivotTablesWithSamePivotCache--) | Restituisce tutte le tabelle pivot con la stessa cache pivot. |
| [getPreserveCellFormattingOnUpdate()](#getPreserveCellFormattingOnUpdate--) | Indica se conservare la formattazione delle celle ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) quando la tabella pivot viene aggiornata o ricalcolata. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Indica se la formattazione delle celle ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) è conservata quando la PivotTable viene aggiornata o ricalcolata. |
| [getPrintDrill()](#getPrintDrill--) | Specifica un valore booleano che indica se gli indicatori di drill devono essere stampati. |
| [getPrintTitles()](#getPrintTitles--) | Indica se i titoli di stampa per il foglio di lavoro sono impostati in base al report PivotTable. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--) | Indica se aggiornare i dati all'apertura del file. |
| [getRefreshDate()](#getRefreshDate--) | Restituisce la data e ora dell'ultimo aggiornamento della PivotTable. |
| [getRefreshedByWho()](#getRefreshedByWho--) | Restituisce il nome dell'ultimo utente che ha aggiornato questa PivotTable. |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--) | Indica se le didascalie degli elementi pivot nell'area riga sono ripetute su ogni pagina stampata per i campi pivot in forma tabellare. |
| [getRowFields()](#getRowFields--) | Restituisce una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) che è attualmente mostrata come campi riga. |
| [getRowGrand()](#getRowGrand--) | Indica se mostrare i totali complessivi per le righe di questa tabella pivot. |
| [getRowHeaderCaption()](#getRowHeaderCaption--) | Restituisce la didascalia personalizzata dell'intestazione di riga in questa PivotTable. |
| [getRowRange()](#getRowRange--) | Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area riga nel report PivotTable. |
| [getSaveData()](#getSaveData--) | Indica se i dati per il report della tabella pivot vengono salvati con la cartella di lavoro. |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--) | Indica se mostrare i totali complessivi per le colonne di questa tabella pivot. |
| [getShowDataTips()](#getShowDataTips--) | Indica se i suggerimenti devono essere visualizzati per le celle dei dati della tabella pivot. |
| [getShowDrill()](#getShowDrill--) | Restituisce se vengono mostrati i pulsanti di espansione/contrazione. |
| [getShowEmptyCol()](#getShowEmptyCol--) | Indica se includere colonne vuote nella tabella |
| [getShowEmptyRow()](#getShowEmptyRow--) | Indica se includere righe vuote nella tabella. |
| [getShowHeaders()](#getShowHeaders--) | Indica se mostrare le didascalie dei campi dati e le didascalie dei campi pivot sull'asse delle righe e sull'asse delle colonne nella visualizzazione della tabella pivot. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--) | Specifica un valore booleano che indica se le informazioni delle proprietà dei membri devono essere omesse dai suggerimenti della tabella pivot. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--) | Indica se l'intestazione della colonna nella tabella pivot deve avere lo stile applicato. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--) | Indica se la formattazione a righe alternate è applicata alla colonna. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--) | Indica se la formattazione della colonna è applicata. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--) | Indica se l'intestazione della riga nella tabella pivot deve avere lo stile applicato. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--) | Indica se la formattazione a righe alternate è applicata alle righe. |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--) | Indica se mostrare i totali complessivi per le righe della tabella pivot. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--) | Indica se la didascalia dell'intestazione della riga è mostrata nel report della tabella pivot. Indica se visualizzare le didascalie dei campi e i menu a discesa dei filtri |
| [getShowValuesRow()](#getShowValuesRow--) | Indica se mostrare la riga dei valori. |
| [getSource()](#getSource--) | Ottieni l'origine dati di questa tabella pivot. |
| [getSource(boolean isOriginal)](#getSource-boolean-) | Ottieni l'origine dati di questa tabella pivot. |
| [getSourceDataConnections()](#getSourceDataConnections--) | Ottiene le origini dati della connessione esterna. |
| [getSourceType()](#getSourceType--) | Ottiene il tipo di origine dati della tabella pivot. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--) | Indica se gli elementi di campo pagina nascosti nel report della tabella pivot sono inclusi nei subtotali di righe e colonne, nei totali di blocco e nei totali complessivi. |
| [getTableRange1()](#getTableRange1--) | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report della tabella pivot, ma non include i campi pagina. |
| [getTableRange2()](#getTableRange2--) | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report della tabella pivot, includendo i campi pagina. |
| [getTag()](#getTag--) | Ottiene una stringa definita dall'utente associata a questa visualizzazione della tabella pivot. |
| [getTopRightArea()](#getTopRightArea--) | Rappresenta l'area vuota in alto a destra della tabella pivot (in alto a sinistra per i fogli RTL). |
| [getValuesField()](#getValuesField--) | Ottiene un oggetto [PivotField](../../com.aspose.cells/pivotfield) che rappresenta tutti i campi dati in una Tabella Pivot. |
| [hasBlankRows()](#hasBlankRows--) | Indica se aggiungere righe vuote. |
| [hashCode()](#hashCode--) |  |
| [isAutoFormat()](#isAutoFormat--) | Indica se il report PivotTable è formattato automaticamente. |
| [isExcel2003Compatible()](#isExcel2003Compatible--) | Specifica se la PivotTable è compatibile con Excel2003 durante l'aggiornamento della PivotTable; se vero, una stringa deve essere lunga al massimo 255 caratteri, quindi se la stringa supera i 255 caratteri verrà troncata. Se falso, la stringa non avrà la restrizione sopra menzionata. |
| [isGridDropZones()](#isGridDropZones--) | Indica se il report PivotTable visualizza il layout classico della pivot. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--) | Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati. |
| [isSelected()](#isSelected--) | Indica se questa PivotTable è selezionata. |
| [move(int row, int column)](#move-int-int-) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [move(String destCellName)](#move-java.lang.String-) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [moveItem(int region, String[] nodes, boolean absolute, int offset)](#moveItem-int-java.lang.String---boolean-int-) | Sposta un elemento su o giù. |
| [moveTo(int row, int column)](#moveTo-int-int-) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [moveTo(int sheetIndex, int row, int column)](#moveTo-int-int-int-) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [moveTo(String destCellName)](#moveTo-java.lang.String-) | Sposta la PivotTable in una posizione diversa nel foglio di lavoro. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Aggiorna [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) dalla fonte dati e calcola i dati e lo stile per la visualizzazione pivot. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Aggiorna [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) dalla fonte dati e calcola i dati e lo stile per la visualizzazione pivot. |
| [refreshData()](#refreshData--) | Aggiorna i dati dalla sua fonte dati alla cache pivot. |
| [refreshData(PivotTableRefreshOption option)](#refreshData-com.aspose.cells.PivotTableRefreshOption-) | Aggiorna i dati e le impostazioni della pivot table dalla sua fonte dati con opzioni. |
| [removeField(int fieldType, PivotField pivotField)](#removeField-int-com.aspose.cells.PivotField-) | Rimuovi il campo dall'area campo specifica |
| [removeField(int fieldType, int baseFieldIndex)](#removeField-int-int-) | Rimuove un campo da una regione pivot specifica. |
| [removeField(int fieldType, String fieldName)](#removeField-int-java.lang.String-) | Rimuove un campo dall'area campo specifica. |
| [selectArea(CellArea ca)](#selectArea-com.aspose.cells.CellArea-) | Seleziona un'area della visualizzazione della pivot table. |
| [setAllowMultipleFiltersPerField(boolean value)](#setAllowMultipleFiltersPerField-boolean-) | Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati. |
| [setAltTextDescription(String value)](#setAltTextDescription-java.lang.String-) | Ottiene la descrizione del testo alternativo. |
| [setAltTextTitle(String value)](#setAltTextTitle-java.lang.String-) | Imposta il titolo del testo alternativo. |
| [setAutoFormat(boolean value)](#setAutoFormat-boolean-) | Indica se il report PivotTable è formattato automaticamente. |
| [setAutoFormatType(int value)](#setAutoFormatType-int-) | Imposta il tipo di formattazione automatica della PivotTable. |
| [setAutofitColumnWidthOnUpdate(boolean value)](#setAutofitColumnWidthOnUpdate-boolean-) | Indica se adattare automaticamente la larghezza della colonna all'aggiornamento |
| [setColumnGrand(boolean value)](#setColumnGrand-boolean-) | Indica se il report della Tabella Pivot mostra i totali generali per le colonne. |
| [setColumnHeaderCaption(String value)](#setColumnHeaderCaption-java.lang.String-) | Imposta la didascalia personalizzata dell'intestazione di colonna della PivotTable. |
| [setCustomListSort(boolean value)](#setCustomListSort-boolean-) | Indica se considerare l'elenco personalizzato integrato durante l'ordinamento dei dati |
| [setDataFieldHeaderName(String value)](#setDataFieldHeaderName-java.lang.String-) | Imposta il nome dell'intestazione del campo dell'area valori nella PivotTable. |
| [setDataSource(String[] value)](#setDataSource-java.lang.String---) | Imposta la fonte dati della pivot table. |
| [setDisplayErrorString(boolean value)](#setDisplayErrorString-boolean-) | Indica se il report della PivotTable visualizza una stringa personalizzata nelle celle che contengono errori. |
| [setDisplayImmediateItems(boolean value)](#setDisplayImmediateItems-boolean-) | Indica se gli elementi nelle aree riga e colonna sono visibili quando l'area dati della PivotTable è vuota. |
| [setDisplayNullString(boolean value)](#setDisplayNullString-boolean-) | Indica se il report della PivotTable visualizza una stringa personalizzata se il valore è nullo. |
| [setEnableDataValueEditing(boolean value)](#setEnableDataValueEditing-boolean-) | Specifica un valore booleano che indica se all'utente è consentito modificare le celle nell'area dati della PivotTable. |
| [setEnableDrilldown(boolean value)](#setEnableDrilldown-boolean-) | Indica se il drilldown è abilitato. |
| [setEnableFieldDialog(boolean value)](#setEnableFieldDialog-boolean-) | Indica se la finestra di dialogo PivotTable Field è disponibile quando l'utente fa doppio clic sul campo della PivotTable. |
| [setEnableFieldList(boolean value)](#setEnableFieldList-boolean-) | Indica se l'elenco dei campi per la PivotTable è disponibile nella visualizzazione di Excel. |
| [setEnableWizard(boolean value)](#setEnableWizard-boolean-) | Indica se la procedura guidata PivotTable è disponibile. |
| [setErrorString(String value)](#setErrorString-java.lang.String-) | Restituisce la stringa visualizzata nelle celle che contengono errori quando la proprietà DisplayErrorString è true. Il valore predefinito è una stringa vuota. |
| [setExcel2003Compatible(boolean value)](#setExcel2003Compatible-boolean-) | Specifica se la PivotTable è compatibile con Excel2003 durante l'aggiornamento della PivotTable; se vero, una stringa deve essere lunga al massimo 255 caratteri, quindi se la stringa supera i 255 caratteri verrà troncata. Se falso, la stringa non avrà la restrizione sopra menzionata. |
| [setFieldListSortAscending(boolean value)](#setFieldListSortAscending-boolean-) | Indica se i campi nella PivotTable sono ordinati in un ordine non predefinito nell'elenco dei campi. |
| [setGrandTotalName(String value)](#setGrandTotalName-java.lang.String-) | Restituisce l'etichetta visualizzata nell'intestazione della colonna o della riga del totale generale. |
| [setGridDropZones(boolean value)](#setGridDropZones-boolean-) | Indica se il report PivotTable visualizza il layout classico della pivot. |
| [setHasBlankRows(boolean value)](#setHasBlankRows-boolean-) | Indica se aggiungere righe vuote. |
| [setIndent(int value)](#setIndent-int-) | Specifica l'incremento di rientro per l'asse compatto e può essere usato per impostare il Layout del report su Forma compatta. |
| [setItemPrintTitles(boolean value)](#setItemPrintTitles-boolean-) | Indica se i nomi di PivotItem devono essere ripetuti nella parte superiore di ogni pagina stampata. |
| [setManualUpdate(boolean value)](#setManualUpdate-boolean-) | Indica se il report della PivotTable viene ricalcolato solo su richiesta dell'utente. |
| [setMergeLabels(boolean value)](#setMergeLabels-boolean-) | Imposta se unire le etichette dei campi riga/colonna che si estendono su più celle. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati. |
| [setMultipleFieldFilters(boolean value)](#setMultipleFieldFilters-boolean-) | Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati. |
| [setName(String value)](#setName-java.lang.String-) | Restituisce il nome della PivotTable |
| [setNullString(String value)](#setNullString-java.lang.String-) | Restituisce la stringa visualizzata nelle celle che contengono valori null quando la proprietà DisplayNullString è true. Il valore predefinito è una stringa vuota. |
| [setPageFieldOrder(int value)](#setPageFieldOrder-int-) | Imposta l'ordine in cui i campi pagina vengono aggiunti al layout del report PivotTable. |
| [setPageFieldWrapCount(int value)](#setPageFieldWrapCount-int-) | Restituisce il numero di campi pagina in ogni colonna o riga del report PivotTable. |
| [setPivotTableStyle(TableStyle value)](#setPivotTableStyle-com.aspose.cells.TableStyle-) | Restituisce le impostazioni di [TableStyle](../../com.aspose.cells/tablestyle) di questa tabella pivot. |
| [setPivotTableStyleName(String value)](#setPivotTableStyleName-java.lang.String-) | Imposta il nome dello stile della pivot table. |
| [setPivotTableStyleType(int value)](#setPivotTableStyleType-int-) | Imposta lo stile predefinito della pivot table. |
| [setPreserveCellFormattingOnUpdate(boolean value)](#setPreserveCellFormattingOnUpdate-boolean-) | Indica se conservare la formattazione delle celle ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) quando la tabella pivot viene aggiornata o ricalcolata. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Indica se la formattazione delle celle ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) è conservata quando la PivotTable viene aggiornata o ricalcolata. |
| [setPrintDrill(boolean value)](#setPrintDrill-boolean-) | Specifica un valore booleano che indica se gli indicatori di drill devono essere stampati. |
| [setPrintTitles(boolean value)](#setPrintTitles-boolean-) | Indica se i titoli di stampa per il foglio di lavoro sono impostati in base al report PivotTable. |
| [setRefreshDataOnOpeningFile(boolean value)](#setRefreshDataOnOpeningFile-boolean-) | Indica se aggiornare i dati all'apertura del file. |
| [setRepeatItemsOnEachPrintedPage(boolean value)](#setRepeatItemsOnEachPrintedPage-boolean-) | Indica se le didascalie degli elementi pivot nell'area riga sono ripetute su ogni pagina stampata per i campi pivot in forma tabellare. |
| [setRowGrand(boolean value)](#setRowGrand-boolean-) | Indica se mostrare i totali complessivi per le righe di questa tabella pivot. |
| [setRowHeaderCaption(String value)](#setRowHeaderCaption-java.lang.String-) | Imposta la didascalia personalizzata dell'intestazione di riga in questa PivotTable. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Indica se i dati per il report della tabella pivot vengono salvati con la cartella di lavoro. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indica se questa PivotTable è selezionata. |
| [setShowColumnGrandTotals(boolean value)](#setShowColumnGrandTotals-boolean-) | Indica se mostrare i totali complessivi per le colonne di questa tabella pivot. |
| [setShowDataTips(boolean value)](#setShowDataTips-boolean-) | Indica se i suggerimenti devono essere visualizzati per le celle dei dati della tabella pivot. |
| [setShowDrill(boolean value)](#setShowDrill-boolean-) | Imposta se mostrare i pulsanti espandi/contrai. |
| [setShowEmptyCol(boolean value)](#setShowEmptyCol-boolean-) | Indica se includere colonne vuote nella tabella |
| [setShowEmptyRow(boolean value)](#setShowEmptyRow-boolean-) | Indica se includere righe vuote nella tabella. |
| [setShowHeaders(boolean value)](#setShowHeaders-boolean-) | Indica se mostrare le didascalie dei campi dati e le didascalie dei campi pivot sull'asse delle righe e sull'asse delle colonne nella visualizzazione della tabella pivot. |
| [setShowMemberPropertyTips(boolean value)](#setShowMemberPropertyTips-boolean-) | Specifica un valore booleano che indica se le informazioni delle proprietà dei membri devono essere omesse dai suggerimenti della tabella pivot. |
| [setShowPivotStyleColumnHeader(boolean value)](#setShowPivotStyleColumnHeader-boolean-) | Indica se l'intestazione della colonna nella tabella pivot deve avere lo stile applicato. |
| [setShowPivotStyleColumnStripes(boolean value)](#setShowPivotStyleColumnStripes-boolean-) | Indica se la formattazione a righe alternate è applicata alla colonna. |
| [setShowPivotStyleLastColumn(boolean value)](#setShowPivotStyleLastColumn-boolean-) | Indica se la formattazione della colonna è applicata. |
| [setShowPivotStyleRowHeader(boolean value)](#setShowPivotStyleRowHeader-boolean-) | Indica se l'intestazione della riga nella tabella pivot deve avere lo stile applicato. |
| [setShowPivotStyleRowStripes(boolean value)](#setShowPivotStyleRowStripes-boolean-) | Indica se la formattazione a righe alternate è applicata alle righe. |
| [setShowRowGrandTotals(boolean value)](#setShowRowGrandTotals-boolean-) | Indica se mostrare i totali complessivi per le righe della tabella pivot. |
| [setShowRowHeaderCaption(boolean value)](#setShowRowHeaderCaption-boolean-) | Indica se la didascalia dell'intestazione della riga è mostrata nel report della tabella pivot. Indica se visualizzare le didascalie dei campi e i menu a discesa dei filtri |
| [setShowValuesRow(boolean value)](#setShowValuesRow-boolean-) | Indica se mostrare la riga dei valori. |
| [setSubtotalHiddenPageItems(boolean value)](#setSubtotalHiddenPageItems-boolean-) | Indica se gli elementi di campo pagina nascosti nel report della tabella pivot sono inclusi nei subtotali di righe e colonne, nei totali di blocco e nei totali complessivi. |
| [setTag(String value)](#setTag-java.lang.String-) | Imposta una stringa definita dall'utente associata a questa visualizzazione della PivotTable. |
| [showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)](#showDetail-int-int-boolean-int-int-) | Mostra i dettagli di un elemento nella regione dati in una nuova tabella. |
| [showInCompactForm()](#showInCompactForm--) | Disposizione della vista PivotTable in forma compatta. |
| [showInOutlineForm()](#showInOutlineForm--) | Disposizione della PivotTable in forma outline. |
| [showInTabularForm()](#showInTabularForm--) | Disposizione della PivotTable in forma tabellare. |
| [showReportFilterPage(PivotField pageField)](#showReportFilterPage-com.aspose.cells.PivotField-) | Mostra tutte le pagine di filtro del report in base a PivotField, il PivotField deve trovarsi nei PageFields. |
| [showReportFilterPageByIndex(int posIndex)](#showReportFilterPageByIndex-int-) | Mostra tutte le pagine di filtro del report in base all'indice di posizione nei PageFields. |
| [showReportFilterPageByName(String fieldName)](#showReportFilterPageByName-java.lang.String-) | Mostra tutte le pagine di filtro del report in base al nome di PivotField, il PivotField deve trovarsi nei PageFields. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedField(String name, String formula) {#addCalculatedField-java.lang.String-java.lang.String-}
```
public void addCalculatedField(String name, String formula)
```


Aggiunge un campo calcolato al campo pivot e lo trascina nell'area dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome del campo calcolato |
| formula | java.lang.String | La formula del campo calcolato. |

### addCalculatedField(String name, String formula, boolean dragToDataArea) {#addCalculatedField-java.lang.String-java.lang.String-boolean-}
```
public void addCalculatedField(String name, String formula, boolean dragToDataArea)
```


Aggiunge un campo calcolato al campo pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome del campo calcolato |
| formula | java.lang.String | La formula del campo calcolato. |
| dragToDataArea | boolean | True, trascina immediatamente questo campo nell'area dati |

### addFieldToArea(int fieldType, PivotField pivotField) {#addFieldToArea-int-com.aspose.cells.PivotField-}
```
public int addFieldToArea(int fieldType, PivotField pivotField)
```


Aggiunge il campo all'area specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). il tipo di area dei campi. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | il campo nei campi di base. |

**Returns:**
int - la posizione del campo nei campi specifici.
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Aggiunge il campo all'area specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Il tipo di area dei campi. |
| baseFieldIndex | int | L'indice nei campi di base. |

**Returns:**
int - La posizione del campo nei campi specifici.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Aggiunge il campo all'area specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Il tipo di area dei campi. |
| fieldName | java.lang.String | Il nome nei campi di base. |

**Returns:**
int - La posizione del campo nei campi specifici. Se non esiste alcun campo con quel nome, restituisce -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Calcola i dati della tabella pivot nelle celle.

**Remarks**

Questo metodo calcola i dati solo con i dati memorizzati nella cache nel [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). Quindi, se desideri calcolare con l'ultima fonte dati, utilizza il metodo [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) per calcolare. Se è stata modificata solo l'impostazione della tabella pivot, è sufficiente [calculateData()](../../com.aspose.cells/pivottable\#calculateData--).

### calculateData(PivotTableCalculateOption option) {#calculateData-com.aspose.cells.PivotTableCalculateOption-}
```
public PivotTable[] calculateData(PivotTableCalculateOption option)
```


Calcola la tabella pivot con opzioni.

**Remarks**

Se [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) è true, questo metodo aggiornerà la cache pivot dalla fonte dati, quindi calcolerà tutte le tabelle pivot basate sulla stessa cache pivot. Altrimenti, verrà effettuato solo il calcolo con i dati memorizzati nella cache pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../../com.aspose.cells/pivottablecalculateoption) | Le opzioni per calcolare la tabella pivot |

**Returns:**
com.aspose.cells.PivotTable[] - Restituisce tutte le tabelle pivot che sono state calcolate. Se [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) è true, tutte le tabelle pivot basate sulla stessa cache pivot verranno calcolate insieme.
### calculateRange() {#calculateRange--}
```
public void calculateRange()
```


Calcola l'intervallo della tabella pivot.

**Remarks**

Se questo metodo non è stato chiamato, potrebbe essere che l'intervallo della tabella pivot non sia corretto.

### changeDataSource(String[] source) {#changeDataSource-java.lang.String---}
```
public void changeDataSource(String[] source)
```


Modifica l'origine dati della tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | java.lang.String[] |  |

### clearAll() {#clearAll--}
```
public void clearAll()
```


Rimuove tutti i campi dalle regioni.

### clearData() {#clearData--}
```
public void clearData()
```


Cancella i dati e la formattazione della vista della tabella pivot.

**Remarks**

Se questo metodo non viene chiamato prima di aggiungere o eliminare PivotField, potrebbe essere che i dati della PivotTable non siano corretti

### clearFilters() {#clearFilters--}
```
public void clearFilters()
```


Cancella tutti i filtri di questa tabella pivot.

### copyStyle(PivotTable pivotTable) {#copyStyle-com.aspose.cells.PivotTable-}
```
public void copyStyle(PivotTable pivotTable)
```


Copia lo stile denominato da un'altra tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Tabella pivot di origine. |

### dispose() {#dispose--}
```
public void dispose()
```


Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportViewToJson(PivotViewToJsonOptions options) {#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-}
```
public String exportViewToJson(PivotViewToJsonOptions options)
```


Esporta la vista pivot come JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [PivotViewToJsonOptions](../../com.aspose.cells/pivotviewtojsonoptions) |  |

**Returns:**
java.lang.String -
### fields(int fieldType) {#fields-int-}
```
public PivotFieldCollection fields(int fieldType)
```


Ottiene i campi specifici per tipo di campo.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.GetFields(PivotFieldType). Questo metodo sarà rimosso 12 mesi dopo, a partire da maggio 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). il tipo di campo. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific field collection
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


Formatta l'area selezionata della Tabella Pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | L'intervallo delle celle. |
| style | [Style](../../com.aspose.cells/style) | Lo stile |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


Formatta l'area selezionata della Tabella Pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | L'area di visualizzazione pivot selezionata. |
| style | [Style](../../com.aspose.cells/style) | L'impostazione formattata. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


Formatta la cella nell'area della tabella pivot

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga della cella |
| colonna | int | Indice della colonna della cella |
| style | [Style](../../com.aspose.cells/style) | Stile utilizzato per formattare la cella |

### formatAll(Style style) {#formatAll-com.aspose.cells.Style-}
```
public void formatAll(Style style)
```


Formatta tutte le celle nell'area della tabella pivot

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Stile utilizzato per formattare |

### formatRow(int row, Style style) {#formatRow-int-com.aspose.cells.Style-}
```
public void formatRow(int row, Style style)
```


Formatta i dati della riga nell'area della tabella pivot

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga dell'oggetto Row |
| style | [Style](../../com.aspose.cells/style) | Stile utilizzato per formattare |

### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```
public boolean getAllowMultipleFiltersPerField()
```


Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati.

**Returns:**
boolean
### getAltTextDescription() {#getAltTextDescription--}
```
public String getAltTextDescription()
```


Ottiene la descrizione del testo alternativo.

**Returns:**
java.lang.String
### getAltTextTitle() {#getAltTextTitle--}
```
public String getAltTextTitle()
```


Ottiene il titolo del testo alternativo.

**Returns:**
java.lang.String
### getAutoFormatType() {#getAutoFormatType--}
```
public int getAutoFormatType()
```


Ottiene il tipo di formato automatico della Tabella Pivot.

Vedi [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Returns:**
int
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```
public boolean getAutofitColumnWidthOnUpdate()
```


Indica se adattare automaticamente la larghezza della colonna all'aggiornamento

**Returns:**
boolean
### getBaseFields() {#getBaseFields--}
```
public PivotFieldCollection getBaseFields()
```


Restituisce tutti i campi pivot di base nella Tabella Pivot.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getButtonArea(int axisType) {#getButtonArea-int-}
```
public CellArea getButtonArea(int axisType)
```


Ottiene l'area che contiene il pulsante del campo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Il tipo di regione. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - 
### getCellByDisplayName(String displayName) {#getCellByDisplayName-java.lang.String-}
```
public Cell getCellByDisplayName(String displayName)
```


Ottiene l'oggetto [Cell](../../com.aspose.cells/cell) per il nome visualizzato del PivotField.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| displayName | java.lang.String | Il DisplayName di PivotField |

**Returns:**
[Cell](../../com.aspose.cells/cell) - the Cell object
### getChildren() {#getChildren--}
```
public PivotTable[] getChildren()
```


Ottiene le tabelle pivot figlie che utilizzano questi dati della Tabella Pivot come origine dati.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotTable.GetDependentPivotTables(). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
com.aspose.cells.PivotTable[] - l'oggetto array PivotTable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnFields() {#getColumnFields--}
```
public PivotFieldCollection getColumnFields()
```


Restituisce un oggetto PivotFields che è attualmente mostrato come campi di colonna.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getColumnGrand() {#getColumnGrand--}
```
public boolean getColumnGrand()
```


Indica se il report della Tabella Pivot mostra i totali generali per le colonne.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotTable.ShowColumnGrandTotals. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```
public String getColumnHeaderCaption()
```


Ottiene la didascalia personalizzata dell'intestazione di colonna della Tabella Pivot.

**Returns:**
java.lang.String
### getColumnRange() {#getColumnRange--}
```
public CellArea getColumnRange()
```


Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area della colonna nel report della PivotTable. Sola lettura.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getConditionalFormats() {#getConditionalFormats--}
```
public PivotConditionalFormatCollection getConditionalFormats()
```


Ottiene i formati condizionali della tabella pivot.

**Returns:**
[PivotConditionalFormatCollection](../../com.aspose.cells/pivotconditionalformatcollection)
### getCustomListSort() {#getCustomListSort--}
```
public boolean getCustomListSort()
```


Indica se considerare l'elenco personalizzato integrato durante l'ordinamento dei dati

**Returns:**
boolean
### getDataBodyRange() {#getDataBodyRange--}
```
public CellArea getDataBodyRange()
```


Restituisce un oggetto [CellArea](../../com.aspose.cells/cellarea) che rappresenta l'intervallo che contiene l'area dei dati nell'elenco tra la riga di intestazione e la riga di inserimento. Sola lettura.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getDataField() {#getDataField--}
```
public PivotField getDataField()
```


Ottiene un oggetto [PivotField](../../com.aspose.cells/pivotfield) che rappresenta tutti i campi dati in una PivotTable. Sola lettura. Verrà creato solo quando ci sono due o più campi dati nella regione Dati. Per impostazione predefinita si trova nella regione delle righe. È possibile trascinarlo nella regione riga/colonna con il metodo PivotTable.AddFieldToArea().

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotTable.ValuesField. Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```
public String getDataFieldHeaderName()
```


Restituisce il nome dell'intestazione del campo dell'area valori nella PivotTable.

**Returns:**
java.lang.String
### getDataFields() {#getDataFields--}
```
public PivotFieldCollection getDataFields()
```


Restituisce una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) che rappresenta tutti i campi dati in una PivotTable.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getDataSource() {#getDataSource--}
```
public String[] getDataSource()
```


Restituisce l'origine dati della PivotTable.

**Returns:**
java.lang.String[]
### getDependentPivotTables() {#getDependentPivotTables--}
```
public PivotTable[] getDependentPivotTables()
```


Restituisce tutte le [PivotTable](../../com.aspose.cells/pivottable) che utilizzano questa PivotTable come origine dati.

**Remarks**

Poiché le tabelle pivot possono dipendere dai dati reciproci, devono essere aggiornate nell'ordine corretto per garantire la coerenza dei dati.

**Returns:**
com.aspose.cells.PivotTable[] -
### getDisplayErrorString() {#getDisplayErrorString--}
```
public boolean getDisplayErrorString()
```


Indica se il report della PivotTable visualizza una stringa personalizzata nelle celle che contengono errori.

**Returns:**
boolean
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```
public boolean getDisplayImmediateItems()
```


Indica se gli elementi nelle aree di riga e colonna sono visibili quando l'area dati della PivotTable è vuota. Il valore predefinito è true.

**Returns:**
boolean
### getDisplayNullString() {#getDisplayNullString--}
```
public boolean getDisplayNullString()
```


Indica se il report della PivotTable visualizza una stringa personalizzata se il valore è nullo.

**Returns:**
boolean
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```
public boolean getEnableDataValueEditing()
```


Specifica un valore booleano che indica se all'utente è consentito modificare le celle nell'area dati della PivotTable. Il valore predefinito è false.

**Returns:**
boolean
### getEnableDrilldown() {#getEnableDrilldown--}
```
public boolean getEnableDrilldown()
```


Indica se il drilldown è abilitato.

**Returns:**
boolean
### getEnableFieldDialog() {#getEnableFieldDialog--}
```
public boolean getEnableFieldDialog()
```


Indica se la finestra di dialogo PivotTable Field è disponibile quando l'utente fa doppio clic sul campo della PivotTable.

**Returns:**
boolean
### getEnableFieldList() {#getEnableFieldList--}
```
public boolean getEnableFieldList()
```


Indica se l'elenco dei campi per la PivotTable è disponibile nella visualizzazione di Excel.

**Returns:**
boolean
### getEnableWizard() {#getEnableWizard--}
```
public boolean getEnableWizard()
```


Indica se la procedura guidata PivotTable è disponibile.

**Returns:**
boolean
### getErrorString() {#getErrorString--}
```
public String getErrorString()
```


Restituisce la stringa visualizzata nelle celle che contengono errori quando la proprietà DisplayErrorString è true. Il valore predefinito è una stringa vuota.

**Returns:**
java.lang.String
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```
public ExternalConnection getExternalConnectionDataSource()
```


Restituisce l'origine dati della connessione esterna.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotTable.GetSourceDataConnections(). Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getFieldListSortAscending() {#getFieldListSortAscending--}
```
public boolean getFieldListSortAscending()
```


Indica se i campi nella PivotTable sono ordinati in un ordine non predefinito nell'elenco dei campi.

**Returns:**
boolean
### getFields(int fieldType) {#getFields-int-}
```
public PivotFieldCollection getFields(int fieldType)
```


Restituisce l'elenco specifico dei campi pivot per regione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). il tipo di regione. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific pivot field collection
### getFilterArea() {#getFilterArea--}
```
public CellArea getFilterArea()
```


Restituisce l'area della regione filtro.

**Remarks**

Valido solo se esistono campi pivot di filtro. Verrà restituita un'area vuota se questa PivotTable non contiene campi pivot di filtro.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getGrandTotalName() {#getGrandTotalName--}
```
public String getGrandTotalName()
```


Restituisce l'etichetta visualizzata nell'intestazione della colonna o della riga del totale generale. Il valore predefinito è la stringa "Grand Total".

**Returns:**
java.lang.String
### getHorizontalBreaks() {#getHorizontalBreaks--}
```
public ArrayList getHorizontalBreaks()
```


Restituisce l'elenco degli indici di riga della tabella pivot per le interruzioni di pagina orizzontali

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotTable.GetHorizontalPageBreaks(). Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.util.ArrayList -
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public int[] getHorizontalPageBreaks()
```


Restituisce le interruzioni di pagina orizzontali di questa tabella pivot.

**Returns:**
int[] -
### getIndent() {#getIndent--}
```
public int getIndent()
```


Specifica l'incremento di rientro per l'asse compatto e può essere usato per impostare il Layout del report su Forma compatta.

**Returns:**
int
### getItemPrintTitles() {#getItemPrintTitles--}
```
public boolean getItemPrintTitles()
```


Indica se i nomi di PivotItem devono essere ripetuti nella parte superiore di ogni pagina stampata.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotTable.RepeatItemsOnEachPrintedPage. Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getManualUpdate() {#getManualUpdate--}
```
public boolean getManualUpdate()
```


Indica se il report della PivotTable viene ricalcolato solo su richiesta dell'utente.

**Returns:**
boolean
### getMergeLabels() {#getMergeLabels--}
```
public boolean getMergeLabels()
```


Restituisce se unire le etichette dei campi riga/colonna che si estendono su più celle.

**Returns:**
boolean
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati.

Vedi [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotCache.MissingItemsLimit. Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Restituisce il nome della PivotTable

**Returns:**
java.lang.String
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
```
public String[] getNamesOfSourceDataConnections()
```


Restituisce i nomi delle connessioni dati di origine esterne.

**Returns:**
java.lang.String[]
### getNullString() {#getNullString--}
```
public String getNullString()
```


Restituisce la stringa visualizzata nelle celle che contengono valori null quando la proprietà DisplayNullString è true. Il valore predefinito è una stringa vuota.

**Returns:**
java.lang.String
### getPageFieldOrder() {#getPageFieldOrder--}
```
public int getPageFieldOrder()
```


Restituisce l'ordine in cui i campi pagina vengono aggiunti al layout del report PivotTable.

Vedi [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```
public int getPageFieldWrapCount()
```


Restituisce il numero di campi pagina in ogni colonna o riga del report PivotTable.

**Returns:**
int
### getPageFields() {#getPageFields--}
```
public PivotFieldCollection getPageFields()
```


Restituisce una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) che è attualmente mostrata come campi pagina.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getPivotCache() {#getPivotCache--}
```
public PivotCache getPivotCache()
```


Restituisce l'origine dati.

**Returns:**
[PivotCache](../../com.aspose.cells/pivotcache)
### getPivotFilters() {#getPivotFilters--}
```
public PivotFilterCollection getPivotFilters()
```


Restituisce tutti i filtri nella tabella pivot.

**Returns:**
[PivotFilterCollection](../../com.aspose.cells/pivotfiltercollection)
### getPivotFormatConditions() {#getPivotFormatConditions--}
```
public PivotFormatConditionCollection getPivotFormatConditions()
```


Restituisce le Condizioni di Formato della tabella pivot.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotTable.ConditionalFormats. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[PivotFormatConditionCollection](../../com.aspose.cells/pivotformatconditioncollection)
### getPivotFormats() {#getPivotFormats--}
```
public PivotTableFormatCollection getPivotFormats()
```


Restituisce tutti i formati cella applicati a questa tabella pivot.

**Returns:**
[PivotTableFormatCollection](../../com.aspose.cells/pivottableformatcollection)
### getPivotTableStyle() {#getPivotTableStyle--}
```
public TableStyle getPivotTableStyle()
```


Restituisce le impostazioni di [TableStyle](../../com.aspose.cells/tablestyle) di questa tabella pivot.

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle)
### getPivotTableStyleName() {#getPivotTableStyleName--}
```
public String getPivotTableStyleName()
```


Restituisce il nome dello stile della tabella pivot.

**Returns:**
java.lang.String
### getPivotTableStyleType() {#getPivotTableStyleType--}
```
public int getPivotTableStyleType()
```


Restituisce lo stile predefinito della tabella pivot.

Vedi [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Returns:**
int
### getPivotTablesWithSamePivotCache() {#getPivotTablesWithSamePivotCache--}
```
public PivotTable[] getPivotTablesWithSamePivotCache()
```


Restituisce tutte le tabelle pivot con la stessa cache pivot.

**Returns:**
com.aspose.cells.PivotTable[] -
### getPreserveCellFormattingOnUpdate() {#getPreserveCellFormattingOnUpdate--}
```
public boolean getPreserveCellFormattingOnUpdate()
```


Indica se conservare la formattazione delle celle ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) quando la tabella pivot viene aggiornata o ricalcolata.

**Returns:**
boolean
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Indica se la formattazione delle celle ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) è conservata quando la PivotTable viene aggiornata o ricalcolata.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotTable.PreserveCellFormattingOnUpdate. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getPrintDrill() {#getPrintDrill--}
```
public boolean getPrintDrill()
```


Specifica un valore booleano che indica se gli indicatori di drill devono essere stampati. Stampa i pulsanti di espansione/collasso quando visualizzati su pivottable.

**Returns:**
boolean
### getPrintTitles() {#getPrintTitles--}
```
public boolean getPrintTitles()
```


Indica se i titoli di stampa per il foglio di lavoro sono impostati in base al report della PivotTable. Il valore predefinito è false.

**Returns:**
boolean
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```
public boolean getRefreshDataOnOpeningFile()
```


Indica se aggiornare i dati all'apertura del file.

**Returns:**
boolean
### getRefreshDate() {#getRefreshDate--}
```
public DateTime getRefreshDate()
```


Restituisce la data e ora dell'ultimo aggiornamento della PivotTable.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getRefreshedByWho() {#getRefreshedByWho--}
```
public String getRefreshedByWho()
```


Restituisce il nome dell'ultimo utente che ha aggiornato questa PivotTable.

**Returns:**
java.lang.String
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```
public boolean getRepeatItemsOnEachPrintedPage()
```


Indica se le didascalie degli elementi pivot nell'area riga sono ripetute su ogni pagina stampata per i campi pivot in forma tabellare.

**Returns:**
boolean
### getRowFields() {#getRowFields--}
```
public PivotFieldCollection getRowFields()
```


Restituisce una [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) che è attualmente mostrata come campi riga.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getRowGrand() {#getRowGrand--}
```
public boolean getRowGrand()
```


Indica se mostrare i totali complessivi per le righe di questa tabella pivot.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotTable.ShowRowGrandTotals. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getRowHeaderCaption() {#getRowHeaderCaption--}
```
public String getRowHeaderCaption()
```


Restituisce la didascalia personalizzata dell'intestazione di riga in questa PivotTable.

**Returns:**
java.lang.String
### getRowRange() {#getRowRange--}
```
public CellArea getRowRange()
```


Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'area di riga nel report della PivotTable. Sola lettura.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Indica se i dati per il report della tabella pivot vengono salvati con la cartella di lavoro.

**Returns:**
boolean
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```
public boolean getShowColumnGrandTotals()
```


Indica se mostrare i totali complessivi per le colonne di questa tabella pivot.

**Returns:**
boolean
### getShowDataTips() {#getShowDataTips--}
```
public boolean getShowDataTips()
```


Indica se i suggerimenti devono essere visualizzati per le celle dei dati della tabella pivot.

**Returns:**
boolean
### getShowDrill() {#getShowDrill--}
```
public boolean getShowDrill()
```


Restituisce se vengono mostrati i pulsanti di espansione/contrazione.

**Returns:**
boolean
### getShowEmptyCol() {#getShowEmptyCol--}
```
public boolean getShowEmptyCol()
```


Indica se includere colonne vuote nella tabella

**Returns:**
boolean
### getShowEmptyRow() {#getShowEmptyRow--}
```
public boolean getShowEmptyRow()
```


Indica se includere righe vuote nella tabella.

**Returns:**
boolean
### getShowHeaders() {#getShowHeaders--}
```
public boolean getShowHeaders()
```


Indica se mostrare le didascalie dei campi dati e le didascalie dei campi pivot sull'asse delle righe e sull'asse delle colonne nella visualizzazione della tabella pivot.

**Returns:**
boolean
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```
public boolean getShowMemberPropertyTips()
```


Specifica un valore booleano che indica se le informazioni delle proprietà dei membri devono essere omesse dai suggerimenti della tabella pivot.

**Returns:**
boolean
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```
public boolean getShowPivotStyleColumnHeader()
```


Indica se l'intestazione della colonna nella tabella pivot deve avere lo stile applicato.

**Returns:**
boolean
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```
public boolean getShowPivotStyleColumnStripes()
```


Indica se la formattazione a righe alternate è applicata alla colonna.

**Returns:**
boolean
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```
public boolean getShowPivotStyleLastColumn()
```


Indica se la formattazione della colonna è applicata.

**Returns:**
boolean
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```
public boolean getShowPivotStyleRowHeader()
```


Indica se l'intestazione della riga nella tabella pivot deve avere lo stile applicato.

**Returns:**
boolean
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```
public boolean getShowPivotStyleRowStripes()
```


Indica se la formattazione a righe alternate è applicata alle righe.

**Returns:**
boolean
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```
public boolean getShowRowGrandTotals()
```


Indica se mostrare i totali complessivi per le righe della tabella pivot.

**Remarks**

**Returns:**
boolean
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```
public boolean getShowRowHeaderCaption()
```


Indica se la didascalia dell'intestazione della riga è mostrata nel report della tabella pivot. Indica se visualizzare le didascalie dei campi e i menu a discesa dei filtri

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotTable.ShowHeaders. Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getShowValuesRow() {#getShowValuesRow--}
```
public boolean getShowValuesRow()
```


Indica se mostrare la riga dei valori.

**Returns:**
boolean
### getSource() {#getSource--}
```
public String[] getSource()
```


Ottieni l'origine dati di questa tabella pivot.

**Returns:**
java.lang.String[]
### getSource(boolean isOriginal) {#getSource-boolean-}
```
public String[] getSource(boolean isOriginal)
```


Ottieni l'origine dati di questa tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isOriginal | boolean | Indica se restituire l'originale o la fonte dati visualizzata. |

**Returns:**
java.lang.String[] -
### getSourceDataConnections() {#getSourceDataConnections--}
```
public ExternalConnection[] getSourceDataConnections()
```


Ottiene le origini dati della connessione esterna.

**Returns:**
com.aspose.cells.ExternalConnection[]
### getSourceType() {#getSourceType--}
```
public byte getSourceType()
```


Ottiene il tipo di origine dati della tabella pivot.

Vedi [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```
public boolean getSubtotalHiddenPageItems()
```


Indica se gli elementi di campo pagina nascosti nel report della PivotTable sono inclusi nei subtotali di riga e colonna, nei totali di blocco e nei totali generali. Il valore predefinito è False.

**Returns:**
boolean
### getTableRange1() {#getTableRange1--}
```
public CellArea getTableRange1()
```


Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report PivotTable, ma non include i campi di pagina. Sola lettura.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTableRange2() {#getTableRange2--}
```
public CellArea getTableRange2()
```


Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report PivotTable, includendo i campi di pagina. Sola lettura.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTag() {#getTag--}
```
public String getTag()
```


Ottiene una stringa definita dall'utente associata a questa visualizzazione della tabella pivot.

**Returns:**
java.lang.String
### getTopRightArea() {#getTopRightArea--}
```
public CellArea getTopRightArea()
```


Rappresenta l'area vuota in alto a destra della tabella pivot (in alto a sinistra per i fogli RTL).

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getValuesField() {#getValuesField--}
```
public PivotField getValuesField()
```


Ottiene un oggetto [PivotField](../../com.aspose.cells/pivotfield) che rappresenta tutti i campi dati in una PivotTable. Sola lettura. Verrà creato solo quando ci sono due o più campi dati nella regione Dati. Per impostazione predefinita si trova nella regione delle righe. È possibile trascinarlo nella regione riga/colonna con il metodo PivotTable.AddFieldToArea().

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### hasBlankRows() {#hasBlankRows--}
```
public boolean hasBlankRows()
```


Indica se aggiungere righe vuote. Questa proprietà si applica solo ai tipi di autoformattazione PivotTable che richiedono l'aggiunta di righe vuote.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare la proprietà PivotField.InsertBlankRow. Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFormat() {#isAutoFormat--}
```
public boolean isAutoFormat()
```


Indica se il report PivotTable è formattato automaticamente. Casella di controllo \"autoformat table\" presente nelle opzioni PivotTable per Excel 2003

**Returns:**
boolean
### isExcel2003Compatible() {#isExcel2003Compatible--}
```
public boolean isExcel2003Compatible()
```


Specifica se la PivotTable è compatibile con Excel2003 durante l'aggiornamento della PivotTable; se true, una stringa deve essere lunga al massimo 255 caratteri, quindi se supera i 255 caratteri verrà troncata. Se false, la stringa non avrà la restrizione suddetta. Il valore predefinito è true.

**Returns:**
boolean
### isGridDropZones() {#isGridDropZones--}
```
public boolean isGridDropZones()
```


Indica se il report PivotTable visualizza il layout classico della pivot. (consente di trascinare i campi nella griglia)

**Returns:**
boolean
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```
public boolean isMultipleFieldFilters()
```


Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare la proprietà PivotTable.AllowMultipleFiltersPerField. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Indica se questa PivotTable è selezionata.

**Returns:**
boolean
### move(int row, int column) {#move-int-int-}
```
public void move(int row, int column)
```


Sposta la PivotTable in una posizione diversa nel foglio di lavoro.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare il metodo PivotTable.MoveTo(). Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | indice di riga. |
| colonna | int | indice di colonna. |

### move(String destCellName) {#move-java.lang.String-}
```
public void move(String destCellName)
```


Sposta la PivotTable in una posizione diversa nel foglio di lavoro.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare il metodo PivotTable.MoveTo(). Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destCellName | java.lang.String | il nome della cella di destinazione. |

### moveItem(int region, String[] nodes, boolean absolute, int offset) {#moveItem-int-java.lang.String---boolean-int-}
```
public void moveItem(int region, String[] nodes, boolean absolute, int offset)
```


Sposta un elemento su o giù.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| region | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). La regione. Solo per riga o colonna. |
| nodi | java.lang.String[] | L'elemento. |
| assoluto | boolean | Indica se l'offset è una posizione assoluta. |
| offset | int | Se absolute è true: 0 sposta all'inizio, -1 sposta alla fine, gli altri indicano una posizione assoluta; altrimenti offset è una posizione relativa. |

### moveTo(int row, int column) {#moveTo-int-int-}
```
public void moveTo(int row, int column)
```


Sposta la PivotTable in una posizione diversa nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | indice di riga. |
| colonna | int | indice di colonna. |

### moveTo(int sheetIndex, int row, int column) {#moveTo-int-int-int-}
```
public void moveTo(int sheetIndex, int row, int column)
```


Sposta la PivotTable in una posizione diversa nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | l'indice del foglio di lavoro di destinazione |
| riga | int | indice di riga. |
| colonna | int | indice di colonna. |

### moveTo(String destCellName) {#moveTo-java.lang.String-}
```
public void moveTo(String destCellName)
```


Sposta la PivotTable in una posizione diversa nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destCellName | java.lang.String | il nome della cella di destinazione. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int refresh()
```


Aggiorna [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) dalla fonte dati e calcola i dati e lo stile per la visualizzazione pivot.

**Remarks**

Tutte le tabelle pivot che dipendono dallo stesso PivotCache saranno ricalcolate.

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Aggiorna [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) dalla fonte dati e calcola i dati e lo stile per la visualizzazione pivot.

**Remarks**

Tutte le tabelle pivot che dipendono dallo stesso PivotCache saranno ricalcolate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refreshData() {#refreshData--}
```
public int refreshData()
```


Aggiorna i dati dalla sua fonte dati alla cache pivot.

**Remarks**

Raccoglieremo i dati dalla fonte dati in una cache pivot, quindi calcoleremo i dati nella cache nelle celle. È consigliabile chiamare semplicemente [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) per aggiornare e calcolare tutte le tabelle pivot nel file, invece di aggiornare una per una. NOTA: Questo metodo è ora obsoleto. Invece, utilizzare il metodo [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) e rimuovere il successivo [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) perché questa tabella pivot verrà calcolata durante l'aggiornamento di [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). Questo metodo sarà rimosso 12 mesi dopo, a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### refreshData(PivotTableRefreshOption option) {#refreshData-com.aspose.cells.PivotTableRefreshOption-}
```
public int refreshData(PivotTableRefreshOption option)
```


Aggiorna i dati e le impostazioni della pivot table dalla sua fonte dati con opzioni.

**Remarks**

Raccoglieremo i dati dalla fonte dati in una cache pivot, quindi calcoleremo i dati nella cache nelle celle. È consigliabile chiamare semplicemente [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) per aggiornare e calcolare tutte le tabelle pivot nel file, invece di aggiornare una per una. NOTA: Questo metodo è ora obsoleto. Invece, utilizzare il metodo [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) e rimuovere il successivo [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) perché questa tabella pivot verrà calcolata durante l'aggiornamento di [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) Questo metodo sarà rimosso 12 mesi dopo, a partire da giugno 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Le opzioni per l'aggiornamento della fonte dati della tabella pivot. |

**Returns:**
int
### removeField(int fieldType, PivotField pivotField) {#removeField-int-com.aspose.cells.PivotField-}
```
public void removeField(int fieldType, PivotField pivotField)
```


Rimuovi il campo dall'area campo specifica

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). il tipo di area dei campi. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | il campo nei campi di base. |

### removeField(int fieldType, int baseFieldIndex) {#removeField-int-int-}
```
public void removeField(int fieldType, int baseFieldIndex)
```


Rimuove un campo da una regione pivot specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Il tipo di area dei campi. |
| baseFieldIndex | int | L'indice del campo nei campi di base. |

### removeField(int fieldType, String fieldName) {#removeField-int-java.lang.String-}
```
public void removeField(int fieldType, String fieldName)
```


Rimuove un campo dall'area campo specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Il tipo di area dei campi. |
| fieldName | java.lang.String | Il nome nei campi di base. |

### selectArea(CellArea ca) {#selectArea-com.aspose.cells.CellArea-}
```
public PivotAreaCollection selectArea(CellArea ca)
```


Seleziona un'area della visualizzazione della pivot table.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | L'area della cella. |

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection) - 
### setAllowMultipleFiltersPerField(boolean value) {#setAllowMultipleFiltersPerField-boolean-}
```
public void setAllowMultipleFiltersPerField(boolean value)
```


Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAltTextDescription(String value) {#setAltTextDescription-java.lang.String-}
```
public void setAltTextDescription(String value)
```


Ottiene la descrizione del testo alternativo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAltTextTitle(String value) {#setAltTextTitle-java.lang.String-}
```
public void setAltTextTitle(String value)
```


Imposta il titolo del testo alternativo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAutoFormat(boolean value) {#setAutoFormat-boolean-}
```
public void setAutoFormat(boolean value)
```


Indica se il report PivotTable è formattato automaticamente. Casella di controllo \"autoformat table\" presente nelle opzioni PivotTable per Excel 2003

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoFormatType(int value) {#setAutoFormatType-int-}
```
public void setAutoFormatType(int value)
```


Imposta il tipo di formattazione automatica della PivotTable.

Vedi [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setAutofitColumnWidthOnUpdate(boolean value) {#setAutofitColumnWidthOnUpdate-boolean-}
```
public void setAutofitColumnWidthOnUpdate(boolean value)
```


Indica se adattare automaticamente la larghezza della colonna all'aggiornamento

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setColumnGrand(boolean value) {#setColumnGrand-boolean-}
```
public void setColumnGrand(boolean value)
```


Indica se il report della Tabella Pivot mostra i totali generali per le colonne.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotTable.ShowColumnGrandTotals. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setColumnHeaderCaption(String value) {#setColumnHeaderCaption-java.lang.String-}
```
public void setColumnHeaderCaption(String value)
```


Imposta la didascalia personalizzata dell'intestazione di colonna della PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCustomListSort(boolean value) {#setCustomListSort-boolean-}
```
public void setCustomListSort(boolean value)
```


Indica se considerare l'elenco personalizzato integrato durante l'ordinamento dei dati

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDataFieldHeaderName(String value) {#setDataFieldHeaderName-java.lang.String-}
```
public void setDataFieldHeaderName(String value)
```


Imposta il nome dell'intestazione del campo dell'area valori nella PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDataSource(String[] value) {#setDataSource-java.lang.String---}
```
public void setDataSource(String[] value)
```


Imposta la fonte dati della pivot table.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String[] |  |

### setDisplayErrorString(boolean value) {#setDisplayErrorString-boolean-}
```
public void setDisplayErrorString(boolean value)
```


Indica se il report della PivotTable visualizza una stringa personalizzata nelle celle che contengono errori.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDisplayImmediateItems(boolean value) {#setDisplayImmediateItems-boolean-}
```
public void setDisplayImmediateItems(boolean value)
```


Indica se gli elementi nelle aree di riga e colonna sono visibili quando l'area dati della PivotTable è vuota. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDisplayNullString(boolean value) {#setDisplayNullString-boolean-}
```
public void setDisplayNullString(boolean value)
```


Indica se il report della PivotTable visualizza una stringa personalizzata se il valore è nullo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableDataValueEditing(boolean value) {#setEnableDataValueEditing-boolean-}
```
public void setEnableDataValueEditing(boolean value)
```


Specifica un valore booleano che indica se all'utente è consentito modificare le celle nell'area dati della PivotTable. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableDrilldown(boolean value) {#setEnableDrilldown-boolean-}
```
public void setEnableDrilldown(boolean value)
```


Indica se il drilldown è abilitato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableFieldDialog(boolean value) {#setEnableFieldDialog-boolean-}
```
public void setEnableFieldDialog(boolean value)
```


Indica se la finestra di dialogo PivotTable Field è disponibile quando l'utente fa doppio clic sul campo della PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableFieldList(boolean value) {#setEnableFieldList-boolean-}
```
public void setEnableFieldList(boolean value)
```


Indica se l'elenco dei campi per la PivotTable è disponibile nella visualizzazione di Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableWizard(boolean value) {#setEnableWizard-boolean-}
```
public void setEnableWizard(boolean value)
```


Indica se la procedura guidata PivotTable è disponibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setErrorString(String value) {#setErrorString-java.lang.String-}
```
public void setErrorString(String value)
```


Restituisce la stringa visualizzata nelle celle che contengono errori quando la proprietà DisplayErrorString è true. Il valore predefinito è una stringa vuota.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setExcel2003Compatible(boolean value) {#setExcel2003Compatible-boolean-}
```
public void setExcel2003Compatible(boolean value)
```


Specifica se la PivotTable è compatibile con Excel2003 durante l'aggiornamento della PivotTable; se true, una stringa deve essere lunga al massimo 255 caratteri, quindi se supera i 255 caratteri verrà troncata. Se false, la stringa non avrà la restrizione suddetta. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFieldListSortAscending(boolean value) {#setFieldListSortAscending-boolean-}
```
public void setFieldListSortAscending(boolean value)
```


Indica se i campi nella PivotTable sono ordinati in un ordine non predefinito nell'elenco dei campi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setGrandTotalName(String value) {#setGrandTotalName-java.lang.String-}
```
public void setGrandTotalName(String value)
```


Restituisce l'etichetta visualizzata nell'intestazione della colonna o della riga del totale generale. Il valore predefinito è la stringa "Grand Total".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setGridDropZones(boolean value) {#setGridDropZones-boolean-}
```
public void setGridDropZones(boolean value)
```


Indica se il report PivotTable visualizza il layout classico della pivot. (consente di trascinare i campi nella griglia)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasBlankRows(boolean value) {#setHasBlankRows-boolean-}
```
public void setHasBlankRows(boolean value)
```


Indica se aggiungere righe vuote. Questa proprietà si applica solo ai tipi di autoformattazione PivotTable che richiedono l'aggiunta di righe vuote.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare la proprietà PivotField.InsertBlankRow. Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIndent(int value) {#setIndent-int-}
```
public void setIndent(int value)
```


Specifica l'incremento di rientro per l'asse compatto e può essere usato per impostare il Layout del report su Forma compatta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setItemPrintTitles(boolean value) {#setItemPrintTitles-boolean-}
```
public void setItemPrintTitles(boolean value)
```


Indica se i nomi di PivotItem devono essere ripetuti nella parte superiore di ogni pagina stampata.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotTable.RepeatItemsOnEachPrintedPage. Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setManualUpdate(boolean value) {#setManualUpdate-boolean-}
```
public void setManualUpdate(boolean value)
```


Indica se il report della PivotTable viene ricalcolato solo su richiesta dell'utente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMergeLabels(boolean value) {#setMergeLabels-boolean-}
```
public void setMergeLabels(boolean value)
```


Imposta se unire le etichette dei campi riga/colonna che si estendono su più celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati.

Vedi [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotCache.MissingItemsLimit. Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMultipleFieldFilters(boolean value) {#setMultipleFieldFilters-boolean-}
```
public void setMultipleFieldFilters(boolean value)
```


Specifica un valore booleano che indica se i campi di una Tabella Pivot possono avere più filtri impostati.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizzare la proprietà PivotTable.AllowMultipleFiltersPerField. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Restituisce il nome della PivotTable

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNullString(String value) {#setNullString-java.lang.String-}
```
public void setNullString(String value)
```


Restituisce la stringa visualizzata nelle celle che contengono valori null quando la proprietà DisplayNullString è true. Il valore predefinito è una stringa vuota.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPageFieldOrder(int value) {#setPageFieldOrder-int-}
```
public void setPageFieldOrder(int value)
```


Imposta l'ordine in cui i campi pagina vengono aggiunti al layout del report PivotTable.

Vedi [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPageFieldWrapCount(int value) {#setPageFieldWrapCount-int-}
```
public void setPageFieldWrapCount(int value)
```


Restituisce il numero di campi pagina in ogni colonna o riga del report PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPivotTableStyle(TableStyle value) {#setPivotTableStyle-com.aspose.cells.TableStyle-}
```
public void setPivotTableStyle(TableStyle value)
```


Restituisce le impostazioni di [TableStyle](../../com.aspose.cells/tablestyle) di questa tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [TableStyle](../../com.aspose.cells/tablestyle) |  |

### setPivotTableStyleName(String value) {#setPivotTableStyleName-java.lang.String-}
```
public void setPivotTableStyleName(String value)
```


Imposta il nome dello stile della pivot table.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPivotTableStyleType(int value) {#setPivotTableStyleType-int-}
```
public void setPivotTableStyleType(int value)
```


Imposta lo stile predefinito della pivot table.

Vedi [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPreserveCellFormattingOnUpdate(boolean value) {#setPreserveCellFormattingOnUpdate-boolean-}
```
public void setPreserveCellFormattingOnUpdate(boolean value)
```


Indica se conservare la formattazione delle celle ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) quando la tabella pivot viene aggiornata o ricalcolata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Indica se la formattazione delle celle ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) è conservata quando la PivotTable viene aggiornata o ricalcolata.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotTable.PreserveCellFormattingOnUpdate. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPrintDrill(boolean value) {#setPrintDrill-boolean-}
```
public void setPrintDrill(boolean value)
```


Specifica un valore booleano che indica se gli indicatori di drill devono essere stampati. Stampa i pulsanti di espansione/collasso quando visualizzati su pivottable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPrintTitles(boolean value) {#setPrintTitles-boolean-}
```
public void setPrintTitles(boolean value)
```


Indica se i titoli di stampa per il foglio di lavoro sono impostati in base al report della PivotTable. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRefreshDataOnOpeningFile(boolean value) {#setRefreshDataOnOpeningFile-boolean-}
```
public void setRefreshDataOnOpeningFile(boolean value)
```


Indica se aggiornare i dati all'apertura del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRepeatItemsOnEachPrintedPage(boolean value) {#setRepeatItemsOnEachPrintedPage-boolean-}
```
public void setRepeatItemsOnEachPrintedPage(boolean value)
```


Indica se le didascalie degli elementi pivot nell'area riga sono ripetute su ogni pagina stampata per i campi pivot in forma tabellare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRowGrand(boolean value) {#setRowGrand-boolean-}
```
public void setRowGrand(boolean value)
```


Indica se mostrare i totali complessivi per le righe di questa tabella pivot.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotTable.ShowRowGrandTotals. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRowHeaderCaption(String value) {#setRowHeaderCaption-java.lang.String-}
```
public void setRowHeaderCaption(String value)
```


Imposta la didascalia personalizzata dell'intestazione di riga in questa PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Indica se i dati per il report della tabella pivot vengono salvati con la cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indica se questa PivotTable è selezionata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowColumnGrandTotals(boolean value) {#setShowColumnGrandTotals-boolean-}
```
public void setShowColumnGrandTotals(boolean value)
```


Indica se mostrare i totali complessivi per le colonne di questa tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowDataTips(boolean value) {#setShowDataTips-boolean-}
```
public void setShowDataTips(boolean value)
```


Indica se i suggerimenti devono essere visualizzati per le celle dei dati della tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowDrill(boolean value) {#setShowDrill-boolean-}
```
public void setShowDrill(boolean value)
```


Imposta se mostrare i pulsanti espandi/contrai.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowEmptyCol(boolean value) {#setShowEmptyCol-boolean-}
```
public void setShowEmptyCol(boolean value)
```


Indica se includere colonne vuote nella tabella

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowEmptyRow(boolean value) {#setShowEmptyRow-boolean-}
```
public void setShowEmptyRow(boolean value)
```


Indica se includere righe vuote nella tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowHeaders(boolean value) {#setShowHeaders-boolean-}
```
public void setShowHeaders(boolean value)
```


Indica se mostrare le didascalie dei campi dati e le didascalie dei campi pivot sull'asse delle righe e sull'asse delle colonne nella visualizzazione della tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowMemberPropertyTips(boolean value) {#setShowMemberPropertyTips-boolean-}
```
public void setShowMemberPropertyTips(boolean value)
```


Specifica un valore booleano che indica se le informazioni delle proprietà dei membri devono essere omesse dai suggerimenti della tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowPivotStyleColumnHeader(boolean value) {#setShowPivotStyleColumnHeader-boolean-}
```
public void setShowPivotStyleColumnHeader(boolean value)
```


Indica se l'intestazione della colonna nella tabella pivot deve avere lo stile applicato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowPivotStyleColumnStripes(boolean value) {#setShowPivotStyleColumnStripes-boolean-}
```
public void setShowPivotStyleColumnStripes(boolean value)
```


Indica se la formattazione a righe alternate è applicata alla colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowPivotStyleLastColumn(boolean value) {#setShowPivotStyleLastColumn-boolean-}
```
public void setShowPivotStyleLastColumn(boolean value)
```


Indica se la formattazione della colonna è applicata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowPivotStyleRowHeader(boolean value) {#setShowPivotStyleRowHeader-boolean-}
```
public void setShowPivotStyleRowHeader(boolean value)
```


Indica se l'intestazione della riga nella tabella pivot deve avere lo stile applicato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowPivotStyleRowStripes(boolean value) {#setShowPivotStyleRowStripes-boolean-}
```
public void setShowPivotStyleRowStripes(boolean value)
```


Indica se la formattazione a righe alternate è applicata alle righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowRowGrandTotals(boolean value) {#setShowRowGrandTotals-boolean-}
```
public void setShowRowGrandTotals(boolean value)
```


Indica se mostrare i totali complessivi per le righe della tabella pivot.

**Remarks**

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowRowHeaderCaption(boolean value) {#setShowRowHeaderCaption-boolean-}
```
public void setShowRowHeaderCaption(boolean value)
```


Indica se la didascalia dell'intestazione della riga è mostrata nel report della tabella pivot. Indica se visualizzare le didascalie dei campi e i menu a discesa dei filtri

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotTable.ShowHeaders. Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowValuesRow(boolean value) {#setShowValuesRow-boolean-}
```
public void setShowValuesRow(boolean value)
```


Indica se mostrare la riga dei valori.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSubtotalHiddenPageItems(boolean value) {#setSubtotalHiddenPageItems-boolean-}
```
public void setSubtotalHiddenPageItems(boolean value)
```


Indica se gli elementi di campo pagina nascosti nel report della PivotTable sono inclusi nei subtotali di riga e colonna, nei totali di blocco e nei totali generali. Il valore predefinito è False.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTag(String value) {#setTag-java.lang.String-}
```
public void setTag(String value)
```


Imposta una stringa definita dall'utente associata a questa visualizzazione della PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn) {#showDetail-int-int-boolean-int-int-}
```
public void showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)
```


Mostra i dettagli di un elemento nella regione dati in una nuova tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | int | Offset alla prima riga di dati nella regione dei dati. |
| columnOffset | int | Offset alla prima colonna di dati nella regione dei dati. |
| newSheet | boolean | Mostra il dettaglio in un nuovo foglio di lavoro. |
| destRow | int | La riga di destinazione. |
| destColumn | int | La colonna di destinazione. |

### showInCompactForm() {#showInCompactForm--}
```
public void showInCompactForm()
```


Disposizione della vista PivotTable in forma compatta.

### showInOutlineForm() {#showInOutlineForm--}
```
public void showInOutlineForm()
```


Disposizione della PivotTable in forma outline.

### showInTabularForm() {#showInTabularForm--}
```
public void showInTabularForm()
```


Disposizione della PivotTable in forma tabellare.

### showReportFilterPage(PivotField pageField) {#showReportFilterPage-com.aspose.cells.PivotField-}
```
public void showReportFilterPage(PivotField pageField)
```


Mostra tutte le pagine di filtro del report in base a PivotField, il PivotField deve trovarsi nei PageFields.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageField | [PivotField](../../com.aspose.cells/pivotfield) | L'oggetto PivotField |

### showReportFilterPageByIndex(int posIndex) {#showReportFilterPageByIndex-int-}
```
public void showReportFilterPageByIndex(int posIndex)
```


Mostra tutte le pagine di filtro del report in base all'indice di posizione nei PageFields.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| posIndex | int | L'indice di posizione nei PageFields |

### showReportFilterPageByName(String fieldName) {#showReportFilterPageByName-java.lang.String-}
```
public void showReportFilterPageByName(String fieldName)
```


Mostra tutte le pagine di filtro del report in base al nome di PivotField, il PivotField deve trovarsi nei PageFields.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldName | java.lang.String | Il nome di PivotField |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

