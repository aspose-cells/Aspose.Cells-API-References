---
title: "PivotField"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un campo in un report PivotTable."
type: docs
url: /it/java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

Rappresenta un campo in un report PivotTable.

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
 
          pivot.calculateData(new PivotTableCalculateOption());
 
         //do your business
 
         book.save("out.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | Aggiungi un elemento di formula calcolata al campo pivot. |
| [clearFilter()](#clearFilter--) | Cancella le impostazioni del filtro su questo campo pivot. |
| [dispose()](#dispose--) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterByDate(int type, DateTime dateTime1, DateTime dateTime2)](#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filtra per valori di data del campo pivot di riga o colonna. |
| [filterByLabel(int type, String label1, String label2)](#filterByLabel-int-java.lang.String-java.lang.String-) | Filtra per didascalie del campo pivot di riga o colonna. |
| [filterByValue(int valueFieldIndex, int type, double value1, double value2)](#filterByValue-int-int-double-double-) | Filtra per valori del campo pivot dei dati. |
| [filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)](#filterTop10-int-int-boolean-int-) | Filtra per valori del campo pivot dei dati. |
| [getAllowDraggingToColumn()](#getAllowDraggingToColumn--) | Indica se il campo specificato può essere trascinato nella regione colonna. |
| [getAllowDraggingToData()](#getAllowDraggingToData--) | Indica se il campo specificato può essere trascinato nella regione valori. |
| [getAllowDraggingToPage()](#getAllowDraggingToPage--) | Indica se il campo specificato può essere trascinato nella regione pagina. |
| [getAllowDraggingToRow()](#getAllowDraggingToRow--) | Indica se il campo specificato può essere trascinato nella regione riga. |
| [getAllowRemovingFromView()](#getAllowRemovingFromView--) | Indica se questo campo pivot può essere rimosso dalla visualizzazione della PivotTable. |
| [getAutoShowCount()](#getAutoShowCount--) | Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato. |
| [getAutoShowField()](#getAutoShowField--) | Rappresenta l'indice del campo auto show. -1 indica il PivotField stesso. |
| [getAutoSortField()](#getAutoSortField--) | Rappresenta l'indice del campo che è ordinato automaticamente |
| [getBaseIndex()](#getBaseIndex--) | Rappresenta l'indice nei campi pivot di origine. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | Ottieni la stringa della formula del campo calcolato specificato. |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | Ottiene l'elemento di pagina attualmente visualizzato per questo campo pivot (solo campo pagina). |
| [getCurrentPageItemText()](#getCurrentPageItemText--) | Ottiene il testo visualizzato dell'elemento di pagina corrente per questo campo pivot (solo campo pagina). |
| [getDisplayName()](#getDisplayName--) | Rappresenta il nome visualizzato del campo pivot nella visualizzazione della tabella pivot. |
| [getDragToColumn()](#getDragToColumn--) | Indica se il campo specificato può essere trascinato nella regione colonna. |
| [getDragToData()](#getDragToData--) | Indica se il campo specificato può essere trascinato nella regione valori. |
| [getDragToHide()](#getDragToHide--) | Indica se questo campo pivot può essere rimosso dalla visualizzazione della PivotTable. |
| [getDragToPage()](#getDragToPage--) | Indica se il campo specificato può essere trascinato nella regione pagina. |
| [getDragToRow()](#getDragToRow--) | Indica se il campo specificato può essere trascinato nella regione riga. |
| [getFilters()](#getFilters--) | Ottiene tutti i filtri pivot applicati a questo campo pivot. |
| [getFormula()](#getFormula--) | Ottiene la formula del campo calcolato. |
| [getFunction()](#getFunction--) | Rappresenta la funzione utilizzata per riepilogare questo campo dati della PivotTable. |
| [getGroupSettings()](#getGroupSettings--) | Ottiene le impostazioni di raggruppamento del campo pivot. |
| [getInsertBlankRow()](#getInsertBlankRow--) | Indica se inserire una riga vuota dopo ogni elemento. |
| [getItemCount()](#getItemCount--) | Ottiene il conteggio degli elementi di base in questo campo pivot. |
| [getItems()](#getItems--) | Ottieni tutte le etichette degli elementi pivot in questo campo. |
| [getMaxValue()](#getMaxValue--) | Ottiene il valore massimo di questo campo. |
| [getMinValue()](#getMinValue--) | Ottiene il valore massimo di questo campo. |
| [getName()](#getName--) | Rappresenta il nome di PivotField. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | Indica se un'operazione di ordinamento che verrà applicata a questo campo pivot è un'operazione di autosort o un semplice ordinamento dei dati. |
| [getNumber()](#getNumber--) | Rappresenta il formato di visualizzazione integrato di numeri e date. |
| [getNumberFormat()](#getNumberFormat--) | Rappresenta il formato di visualizzazione personalizzato di numeri e date. |
| [getOriginalItems()](#getOriginalItems--) | Ottieni gli elementi di base originali; |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | Ottiene il filtro pivot del campo pivot per tipo |
| [getPivotFilters()](#getPivotFilters--) | Ottiene i filtri pivot del campo pivot |
| [getPivotItems()](#getPivotItems--) | Ottiene gli elementi pivot del campo pivot |
| [getPosition()](#getPosition--) | Rappresenta l'indice di [PivotField](../../com.aspose.cells/pivotfield) nella regione. |
| [getRegionType()](#getRegionType--) | Specifica la regione della tabella pivot in cui questo campo è visualizzato. |
| [getShowAllItems()](#getShowAllItems--) | Indica se visualizzare tutti gli elementi nella vista PivotTable, anche se non contengono dati di riepilogo. |
| [getShowCompact()](#getShowCompact--) | Indica se visualizzare le etichette del campo successivo nella stessa colonna nella vista della Tabella Pivot. |
| [getShowInCompactForm()](#getShowInCompactForm--) | Ottiene un valore che indica se questo campo riga utilizza il layout a forma compatta. |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | Ottiene un valore che indica se questo campo riga utilizza il layout a contorno. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | Indica se visualizzare i subtotali in cima o in fondo agli elementi. |
| [getShowValuesSetting()](#getShowValuesSetting--) | Ottiene le impostazioni per la visualizzazione dei valori quando è in uso il calcolo ShowDataAs. |
| [getSortSetting()](#getSortSetting--) | Ottiene tutte le impostazioni dell'ordinamento automatico |
| [getSubtotals()](#getSubtotals--) | Ottiene i subtotali del campo. |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | Indica se mostrare il subtotale specificato per questo campo pivot. |
| [getTop10AutoShowSettings()](#getTop10AutoShowSettings--) | Ottiene le impostazioni Top 10 AutoShow per un campo pivot. |
| [group()](#group--) | Raggruppa automaticamente il campo. |
| [group(PivotFieldGroupOptions options)](#group-com.aspose.cells.PivotFieldGroupOptions-) | Raggruppa il campo pivot con opzioni. |
| [groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-) | Raggruppa il file per i tipi di gruppo data. |
| [groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)](#groupBy-boolean-double-boolean-double-double-boolean-) | Raggruppa il file per numero. |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | Raggruppa il campo in modo personalizzato. |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | Raggruppa il file per i tipi di gruppo data. |
| [groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-) | Raggruppa il campo in modo personalizzato. |
| [groupBy(double interval, boolean newField)](#groupBy-double-boolean-) | Raggruppa automaticamente il campo con intervallo |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | Raggruppa il file per numero. |
| [groupBy(int[] groups, double interval, boolean newField)](#groupBy-int---double-boolean-) | Raggruppa automaticamente il campo con interno |
| [hashCode()](#hashCode--) |  |
| [hideAllDetails()](#hideAllDetails--) | Nasconde tutti i dettagli di ogni elemento pivot. |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | Imposta se il dettaglio di tutti i PivotItem in un campo pivot è nascosto. |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | Imposta se lo specifico PivotItem in un campo dati è nascosto. |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | Imposta se lo specifico PivotItem in un campo dati è nascosto. |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | Imposta se il dettaglio dello specifico PivotItem in un campo pivot è nascosto. |
| [initPivotItems()](#initPivotItems--) | Inizializza gli elementi pivot del campo pivot |
| [isAscendShow()](#isAscendShow--) | Indica se il campo PivotTable specificato è mostrato automaticamente in ordine ascendente. |
| [isAscendSort()](#isAscendSort--) | Indica se gli elementi di questo campo pivot sono ordinati automaticamente in modo ascendente. |
| [isAutoShow()](#isAutoShow--) | Indica se il campo PivotTable specificato è mostrato automaticamente. |
| [isAutoSort()](#isAutoSort--) | Indica se gli elementi di questo campo PivotTable sono ordinati automaticamente. |
| [isAutoSubtotals()](#isAutoSubtotals--) | Indica se il campo specificato mostra subtotali automatici. |
| [isCalculatedField()](#isCalculatedField--) | Indica se questo campo pivot è un campo calcolato. |
| [isHiddenItem(int index)](#isHiddenItem-int-) | Indica se lo specifico PivotItem è nascosto. |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | Indica se nascondere il dettaglio dello specifico PivotItem.. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | Indica se includere nuovi elementi nel campo nel filtro manuale. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | Indica se inserire interruzioni di pagina dopo ogni elemento. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | Indica se è possibile selezionare più elementi nel campo pagina. |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | Indica se ripetere le etichette del campo nella regione riga o colonna. |
| [isValueFields()](#isValueFields--) | Indica se questo campo rappresenta campi valori. |
| [isValuesField()](#isValuesField--) | Indica se questo campo rappresenta un campo valore. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDraggingToColumn(boolean value)](#setAllowDraggingToColumn-boolean-) | Indica se il campo specificato può essere trascinato nella regione colonna. |
| [setAllowDraggingToData(boolean value)](#setAllowDraggingToData-boolean-) | Indica se il campo specificato può essere trascinato nella regione valori. |
| [setAllowDraggingToPage(boolean value)](#setAllowDraggingToPage-boolean-) | Indica se il campo specificato può essere trascinato nella regione pagina. |
| [setAllowDraggingToRow(boolean value)](#setAllowDraggingToRow-boolean-) | Indica se il campo specificato può essere trascinato nella regione riga. |
| [setAllowRemovingFromView(boolean value)](#setAllowRemovingFromView-boolean-) | Indica se questo campo pivot può essere rimosso dalla visualizzazione della PivotTable. |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | Indica se il campo PivotTable specificato è mostrato automaticamente in ordine ascendente. |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Indica se gli elementi di questo campo pivot sono ordinati automaticamente in modo ascendente. |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Indica se il campo PivotTable specificato è mostrato automaticamente. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato. |
| [setAutoShowField(int value)](#setAutoShowField-int-) | Rappresenta l'indice del campo auto show. -1 indica il PivotField stesso. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Indica se gli elementi di questo campo PivotTable sono ordinati automaticamente. |
| [setAutoSortField(int value)](#setAutoSortField-int-) | Rappresenta l'indice del campo che è ordinato automaticamente |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | Indica se il campo specificato mostra subtotali automatici. |
| [setBaseIndex(int value)](#setBaseIndex-int-) | Rappresenta l'indice nei campi pivot di origine. |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | Imposta l'elemento di pagina attualmente visualizzato per questo campo pivot (solo campo pagina). |
| [setCurrentPageItemText(String value)](#setCurrentPageItemText-java.lang.String-) | Ottiene il testo visualizzato dell'elemento di pagina corrente per questo campo pivot (solo campo pagina). |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Rappresenta il nome visualizzato del campo pivot nella visualizzazione della tabella pivot. |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | Indica se il campo specificato può essere trascinato nella regione colonna. |
| [setDragToData(boolean value)](#setDragToData-boolean-) | Indica se il campo specificato può essere trascinato nella regione valori. |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | Indica se questo campo pivot può essere rimosso dalla visualizzazione della PivotTable. |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | Indica se il campo specificato può essere trascinato nella regione pagina. |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | Indica se il campo specificato può essere trascinato nella regione riga. |
| [setFunction(int value)](#setFunction-int-) | Rappresenta la funzione utilizzata per riepilogare questo campo dati della PivotTable. |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | Indica se includere nuovi elementi nel campo nel filtro manuale. |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | Indica se inserire una riga vuota dopo ogni elemento. |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | Indica se inserire interruzioni di pagina dopo ogni elemento. |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | Indica se è possibile selezionare più elementi nel campo pagina. |
| [setName(String value)](#setName-java.lang.String-) | Rappresenta il nome di PivotField. |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | Indica se un'operazione di ordinamento che verrà applicata a questo campo pivot è un'operazione di autosort o un semplice ordinamento dei dati. |
| [setNumber(int value)](#setNumber-int-) | Rappresenta il formato di visualizzazione integrato di numeri e date. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Rappresenta il formato di visualizzazione personalizzato di numeri e date. |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | Indica se ripetere le etichette del campo nella regione riga o colonna. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Indica se visualizzare tutti gli elementi nella vista PivotTable, anche se non contengono dati di riepilogo. |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | Indica se visualizzare le etichette del campo successivo nella stessa colonna nella vista della Tabella Pivot. |
| [setShowInCompactForm(boolean value)](#setShowInCompactForm-boolean-) | Imposta un valore che indica se questo campo riga utilizza il layout a forma compatta. |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | Imposta un valore che indica se questo campo riga utilizza il layout a contorno. |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | Indica se visualizzare i subtotali in cima o in fondo agli elementi. |
| [setSubtotals(int value)](#setSubtotals-int-) | Imposta i subtotali del campo. |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Imposta come subtotale il campo specificato. |
| [showAllDetails()](#showAllDetails--) | Mostra tutti i dettagli di ciascun elemento pivot. |
| [showValuesAs(int showValuesAsType, int baseField, int baseItem)](#showValuesAs-int-int-int-) | Imposta il calcolo "Mostra valori come" per questo campo pivot. |
| [showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)](#showValuesAs-int-int-int-int-) | Mostra i valori del campo dati in un formato di visualizzazione diverso quando è in uso il calcolo ShowDataAs. |
| [showValuesAs(int showValuesAsType, String baseField, String baseItem)](#showValuesAs-int-java.lang.String-java.lang.String-) | Configura il calcolo "Mostra valori come" per questo campo dati. |
| [sortBy(int sortType)](#sortBy-int-) | Ordina questo campo pivot. |
| [sortBy(int sortType, int fieldSortedBy)](#sortBy-int-int-) | Ordina questo campo pivot. |
| [sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)](#sortBy-int-int-int-java.lang.String-) | Ordina questo campo pivot. |
| [sortBy(int sortType, int fieldSortedBy, String cellName)](#sortBy-int-int-java.lang.String-) | Ordina questo campo pivot. |
| [toString()](#toString--) |  |
| [top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)](#top10AutoShow-boolean-boolean-int-int-) | Configura le impostazioni Top10 AutoShow per questo campo pivot. |
| [ungroup()](#ungroup--) | Annulla il raggruppamento del campo pivot. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


Aggiungi un elemento di formula calcolata al campo pivot.

**Remarks**

Supporta solo l'aggiunta di un elemento calcolato al campo Riga/Colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome dell'elemento. |
| formula | java.lang.String | La formula dell'elemento pivot. |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Cancella le impostazioni del filtro su questo campo pivot.

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
### filterByDate(int type, DateTime dateTime1, DateTime dateTime2) {#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter filterByDate(int type, DateTime dateTime1, DateTime dateTime2)
```


Filtra per valori di data del campo pivot di riga o colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Il tipo di filtraggio dei dati. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | L'etichetta della data della condizione di filtro |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | L'etichetta della data limite superiore della condizione di filtro between |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByLabel(int type, String label1, String label2) {#filterByLabel-int-java.lang.String-java.lang.String-}
```
public PivotFilter filterByLabel(int type, String label1, String label2)
```


Filtra per didascalie del campo pivot di riga o colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Il tipo di filtraggio dei dati. |
| label1 | java.lang.String | L'etichetta della condizione di filtro |
| label2 | java.lang.String | L'etichetta di limite superiore della condizione di filtro tra |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByValue(int valueFieldIndex, int type, double value1, double value2) {#filterByValue-int-int-double-double-}
```
public PivotFilter filterByValue(int valueFieldIndex, int type, double value1, double value2)
```


Filtra per valori del campo pivot dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valueFieldIndex | int | L'indice del campo valore nella regione valore. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Il tipo di filtraggio dei dati. |
| value1 | double | Il valore della condizione di filtro |
| value2 | double | Il valore di limite superiore della condizione di filtro tra |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount) {#filterTop10-int-int-boolean-int-}
```
public PivotFilter filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filtra per valori del campo pivot dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valueFieldIndex | int | L'indice del campo dati nella regione dati. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Il tipo di filtraggio dei dati. Può essere solo Count, Sum e Percent. |
| isTop | boolean | Indica se il filtro è dal superiore o dal inferiore |
| itemCount | int | Il numero di elementi |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getAllowDraggingToColumn() {#getAllowDraggingToColumn--}
```
public boolean getAllowDraggingToColumn()
```


Indica se il campo specificato può essere trascinato nella regione colonna. Il valore predefinito è true.

**Returns:**
boolean
### getAllowDraggingToData() {#getAllowDraggingToData--}
```
public boolean getAllowDraggingToData()
```


Indica se il campo specificato può essere trascinato nella regione valori. Il valore predefinito è true.

**Returns:**
boolean
### getAllowDraggingToPage() {#getAllowDraggingToPage--}
```
public boolean getAllowDraggingToPage()
```


Indica se il campo specificato può essere trascinato nella regione pagina. Il valore predefinito è true.

**Returns:**
boolean
### getAllowDraggingToRow() {#getAllowDraggingToRow--}
```
public boolean getAllowDraggingToRow()
```


Indica se il campo specificato può essere trascinato nella regione riga. Il valore predefinito è true.

**Returns:**
boolean
### getAllowRemovingFromView() {#getAllowRemovingFromView--}
```
public boolean getAllowRemovingFromView()
```


Indica se questo campo pivot può essere rimosso dalla visualizzazione della tabella pivot. Il valore predefinito è true.

**Returns:**
boolean
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.AutoShowCount o il metodo PivotField.Top10AutoShow() . Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
int
### getAutoShowField() {#getAutoShowField--}
```
public int getAutoShowField()
```


Rappresenta l'indice del campo auto‑show. -1 indica il PivotField stesso. Deve essere l'indice dei campi dati.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.RankBy o il metodo PivotField.Top10AutoShow() . Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
int
### getAutoSortField() {#getAutoSortField--}
```
public int getAutoSortField()
```


Rappresenta l'indice del campo che è ordinato automaticamente. -1 indica il PivotField stesso, altri valori indicano la posizione dei campi dati.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.SortSetting.SortBy o il metodo PivotField.SortBy() . Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


Rappresenta l'indice nei campi pivot di origine.

**Remarks**

NOTA: Questo setter di questa proprietà è ora obsoleto. Questo setter sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


Ottieni la stringa della formula del campo calcolato specificato.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.GetFormula(). Questo metodo sarà rimosso 12 mesi dopo, a partire da agosto 2024. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPageItem() {#getCurrentPageItem--}
```
public short getCurrentPageItem()
```


Ottiene l'elemento di pagina attualmente visualizzato per questo campo pivot (solo campo pagina).

**Remarks**

Utilizzare [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) come valore sentinella per indicare \"Select All\". Questo è un marcatore predefinito e non è un indice di elemento valido.

**Returns:**
short
### getCurrentPageItemText() {#getCurrentPageItemText--}
```
public String getCurrentPageItemText()
```


Ottiene il testo visualizzato dell'elemento di pagina corrente per questo campo pivot (solo campo pagina).

**Remarks**

Restituisce \"(All)\" quando [getCurrentPageItem()](../../com.aspose.cells/pivotfield\\#getCurrentPageItem--) è uguale a [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX). Per altri valori, restituisce la rappresentazione stringa dell'indice dell'elemento.

**Returns:**
java.lang.String
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Rappresenta il nome visualizzato del campo pivot nella visualizzazione della tabella pivot.

**Returns:**
java.lang.String
### getDragToColumn() {#getDragToColumn--}
```
public boolean getDragToColumn()
```


Indica se il campo specificato può essere trascinato nella regione colonna. Il valore predefinito è true.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToColumn. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
boolean
### getDragToData() {#getDragToData--}
```
public boolean getDragToData()
```


Indica se il campo specificato può essere trascinato nella regione valori. Il valore predefinito è true.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToData. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


Indica se questo campo pivot può essere rimosso dalla visualizzazione della tabella pivot. Il valore predefinito è true.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowRemovingFromView. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
boolean
### getDragToPage() {#getDragToPage--}
```
public boolean getDragToPage()
```


Indica se il campo specificato può essere trascinato nella regione pagina. Il valore predefinito è true.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToPage. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
boolean
### getDragToRow() {#getDragToRow--}
```
public boolean getDragToRow()
```


Indica se il campo specificato può essere trascinato nella regione riga. Il valore predefinito è true.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToRow. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
boolean
### getFilters() {#getFilters--}
```
public PivotFilter[] getFilters()
```


Ottiene tutti i filtri pivot applicati a questo campo pivot.

**Returns:**
com.aspose.cells.PivotFilter[]
### getFormula() {#getFormula--}
```
public String getFormula()
```


Restituisce la formula del campo calcolato. Funziona solo per il campo calcolato.

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


Rappresenta la funzione utilizzata per riepilogare questo campo dati della PivotTable.

Vedi [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


Ottiene le impostazioni di raggruppamento del campo pivot.

**Remarks**

Se questo campo non è raggruppato, verrà restituito Null.

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


Indica se inserire una riga vuota dopo ogni elemento. Solo per i campi di riga.

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


Ottiene il conteggio degli elementi di base in questo campo pivot.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems.Count. Questo metodo sarà rimosso 12 mesi dopo, a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


Ottieni tutte le etichette degli elementi pivot in questo campo.

**Returns:**
java.lang.String[]
### getMaxValue() {#getMaxValue--}
```
public CellValue getMaxValue()
```


Ottiene il valore massimo di questo campo.

**Remarks**

Funziona solo per i campi di riga o colonna il cui valore deve essere data/ora, numero o vuoto.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getMinValue() {#getMinValue--}
```
public CellValue getMinValue()
```


Ottiene il valore massimo di questo campo.

**Remarks**

Funziona solo per i campi di riga o colonna il cui valore deve essere data/ora, numero o vuoto.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getName() {#getName--}
```
public String getName()
```


Rappresenta il nome di PivotField.

**Returns:**
java.lang.String
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```
public boolean getNonAutoSortDefault()
```


Indica se un'operazione di ordinamento che verrà applicata a questo campo pivot è un'operazione di autosort o un semplice ordinamento dei dati.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà !PivotField.SortSetting.IsSimpleSort. Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
boolean
### getNumber() {#getNumber--}
```
public int getNumber()
```


Rappresenta il formato di visualizzazione integrato di numeri e date.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Rappresenta il formato di visualizzazione personalizzato di numeri e date.

**Returns:**
java.lang.String
### getOriginalItems() {#getOriginalItems--}
```
public String[] getOriginalItems()
```


Ottieni gli elementi di base originali;

**Returns:**
java.lang.String[]
### getPivotFilterByType(int type) {#getPivotFilterByType-int-}
```
public PivotFilter getPivotFilterByType(int type)
```


Ottiene il filtro pivot del campo pivot per tipo

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tipo | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getPivotFilters() {#getPivotFilters--}
```
public ArrayList getPivotFilters()
```


Ottiene i filtri pivot del campo pivot

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.GetFilters(). Questo metodo sarà rimosso 12 mesi dopo a partire da novembre 2023. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
java.util.ArrayList
### getPivotItems() {#getPivotItems--}
```
public PivotItemCollection getPivotItems()
```


Ottiene gli elementi pivot del campo pivot

**Returns:**
[PivotItemCollection](../../com.aspose.cells/pivotitemcollection)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Rappresenta l'indice di [PivotField](../../com.aspose.cells/pivotfield) nella regione.

**Returns:**
int
### getRegionType() {#getRegionType--}
```
public int getRegionType()
```


Specifica la regione della tabella pivot in cui questo campo è visualizzato.

Vedi [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Indica se visualizzare tutti gli elementi nella vista PivotTable, anche se non contengono dati di riepilogo. Il valore predefinito è false.

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


Indica se visualizzare le etichette del campo successivo nella stessa colonna nella vista Pivot Table. Solo per i campi di riga.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.ShowInCompactForm. Questo metodo sarà rimosso 12 mesi dopo a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
boolean
### getShowInCompactForm() {#getShowInCompactForm--}
```
public boolean getShowInCompactForm()
```


Restituisce un valore che indica se questo campo di riga utilizza il layout a forma compatta. Valido solo per i campi di riga.

**Remarks**

La forma compatta è una sotto-modalità del layout a contorno. Questa impostazione ha effetto solo quando [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) è true.

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


Restituisce un valore che indica se questo campo di riga utilizza il layout a contorno. Valido solo per i campi di riga.

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


Indica se visualizzare i subtotali in cima o in fondo agli elementi.

**Remarks**

Funziona solo per i campi pivot nella regione di riga quando ShowInOutlineForm è true.

**Returns:**
boolean
### getShowValuesSetting() {#getShowValuesSetting--}
```
public PivotShowValuesSetting getShowValuesSetting()
```


Ottiene le impostazioni per la visualizzazione dei valori quando è in uso il calcolo ShowDataAs.

**Returns:**
[PivotShowValuesSetting](../../com.aspose.cells/pivotshowvaluessetting)
### getSortSetting() {#getSortSetting--}
```
public PivotFieldSortSetting getSortSetting()
```


Ottiene tutte le impostazioni dell'ordinamento automatico

**Returns:**
[PivotFieldSortSetting](../../com.aspose.cells/pivotfieldsortsetting)
### getSubtotals() {#getSubtotals--}
```
public int getSubtotals()
```


Restituisce i subtotali del campo. Solo per i campi pivot di riga o colonna.

Vedi [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Example**

```
         //No subtotals
         rowField.setSubtotals(PivotFieldSubtotalType.NONE);
         //Automatic subtotals
         //rowField.Subtotals = PivotFieldSubtotalType.Automatic;
         //Single subtotals: Sum
         //rowField.Subtotals = PivotFieldSubtotalType.Sum;
         //Multipl subtotals: Sum and count numbers 
         //rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

**Returns:**
int
### getSubtotals(int subtotalType) {#getSubtotals-int-}
```
public boolean getSubtotals(int subtotalType)
```


Indica se mostrare il subtotale specificato per questo campo pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Tipo di subtotale. |

**Returns:**
boolean - Restituisce se mostra il subtotale specificato.
### getTop10AutoShowSettings() {#getTop10AutoShowSettings--}
```
public PivotFieldTop10AutoShowSettings getTop10AutoShowSettings()
```


Ottiene le impostazioni Top 10 AutoShow per un campo pivot.

**Returns:**
[PivotFieldTop10AutoShowSettings](../../com.aspose.cells/pivotfieldtop10autoshowsettings)
### group() {#group--}
```
public boolean group()
```


Raggruppa automaticamente il campo.

**Remarks**

Se il campo contiene solo valori vuoti e data/ora, il campo sarà raggruppato per Mesi. Se il campo contiene solo valori vuoti e numeri, il campo sarà raggruppato per Numeri. Altrimenti restituisce solo false senza alcun raggruppamento.

**Returns:**
boolean
### group(PivotFieldGroupOptions options) {#group-com.aspose.cells.PivotFieldGroupOptions-}
```
public boolean group(PivotFieldGroupOptions options)
```


Raggruppa il campo pivot con opzioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [PivotFieldGroupOptions](../../com.aspose.cells/pivotfieldgroupoptions) | Opzioni per le impostazioni di raggruppamento del campo pivot. |

**Returns:**
boolean -
### groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Raggruppa il file per i tipi di gruppo data.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isAutoStart | boolean | Indica se rilevare automaticamente il valore della data/ora di inizio. |
| start | [DateTime](../../com.aspose.cells/datetime) | La data/ora di inizio |
| isAutoEnd | boolean | Indica se rilevare automaticamente il valore della data/ora di fine. |
| end | [DateTime](../../com.aspose.cells/datetime) | La data/ora di fine |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Tipi di raggruppamento |
| intervallo | double | L'intervallo |
| firstAsNewField | boolean | Indica se aggiungere un nuovo campo alla pivot table. Solo per il primo elemento del gruppo. |

**Returns:**
boolean - False significa che questo campo non può essere raggruppato per data e ora.
### groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField) {#groupBy-boolean-double-boolean-double-double-boolean-}
```
public boolean groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)
```


Raggruppa il file per numero.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isAutoStart | boolean | Indica se rilevare automaticamente il valore di inizio. |
| inizio | double | Il valore di inizio |
| isAutoEnd | boolean | Indica se rilevare automaticamente il valore di fine. |
| fine | double | Il valore di fine |
| intervallo | double | L'intervallo |
| newField | boolean | Indica se aggiungere un nuovo campo alla tabella pivot |

**Returns:**
boolean - False significa che questo campo non può essere raggruppato per data e ora.
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public boolean groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


Raggruppa il campo in modo personalizzato.

**Remarks**

NOTE: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions options) con la proprietà PivotFieldGroupOptions.DiscreteGroupItems. Questo metodo sarà rimosso tra 6 mesi a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | Gli elementi del gruppo personalizzato. |
| newField | boolean | Indica se aggiungere un nuovo campo alla tabella pivot |

**Returns:**
boolean - False significa che questo campo non può essere raggruppato per data e ora.
### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Raggruppa il file per i tipi di gruppo data.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | La data/ora di inizio |
| end | [DateTime](../../com.aspose.cells/datetime) | La data/ora di fine |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Tipi di raggruppamento |
| intervallo | double | L'intervallo |
| firstAsNewField | boolean | Indica se aggiungere un nuovo campo alla pivot table. Solo per il primo elemento del gruppo. |

**Returns:**
boolean - False significa che questo campo non può essere raggruppato per data e ora.
### groupBy(DiscreteGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-}
```
public boolean groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)
```


Raggruppa il campo in modo personalizzato.

**Remarks**

NOTE: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions options) con la proprietà PivotFieldGroupOptions.DiscreteGroupItems. Questo metodo sarà rimosso tra 6 mesi a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customGroupItems | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) | Gli elementi del gruppo personalizzato. |
| newField | boolean | Indica se aggiungere un nuovo campo alla tabella pivot |

**Returns:**
boolean -
### groupBy(double interval, boolean newField) {#groupBy-double-boolean-}
```
public void groupBy(double interval, boolean newField)
```


Raggruppa automaticamente il campo con intervallo

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | double | L'interno del gruppo. Un valore automatico verrà assegnato se è zero, |
| newField | boolean | Indica se aggiungere un nuovo campo alla tabella pivot. Solo per il raggruppamento DateTime. |

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public boolean groupBy(double start, double end, double interval, boolean newField)
```


Raggruppa il file per numero.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | double | Il valore di inizio |
| fine | double | Il valore di fine |
| intervallo | double | L'intervallo |
| newField | boolean | Indica se aggiungere un nuovo campo alla tabella pivot |

**Returns:**
boolean - False significa che questo campo non può essere raggruppato per data e ora.
### groupBy(int[] groups, double interval, boolean newField) {#groupBy-int---double-boolean-}
```
public void groupBy(int[] groups, double interval, boolean newField)
```


Raggruppa automaticamente il campo con interno

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Tipi di raggruppamento |
| intervallo | double | L'interno del gruppo. Un valore automatico verrà assegnato se è zero, funziona solo per il raggruppamento per Numeri o Giorni. |
| newField | boolean | Indica se aggiungere un nuovo campo alla tabella pivot. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideAllDetails() {#hideAllDetails--}
```
public void hideAllDetails()
```


Nasconde tutti i dettagli di ogni elemento pivot.

### hideDetail(boolean isHiddenDetail) {#hideDetail-boolean-}
```
public void hideDetail(boolean isHiddenDetail)
```


Imposta se i dettagli di tutti i PivotItems in un campo pivot sono nascosti. Cioè comprime/espande questo campo.

**Remarks**

NOTE: Questo metodo è ora obsoleto. Invece, si prega di utilizzare i metodi PivotItemsCollection.HideAllDetails() e UnhideAllDetails(). Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isHiddenDetail | boolean | Indica se nascondere il dettaglio del campo pivot. |

### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


Imposta se lo specifico PivotItem in un campo dati è nascosto.

**Remarks**

NOTE: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems[int].IsHidden. Questo metodo sarà rimosso tra 12 mesi a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | l'indice del pivotItem nel pivotField. |
| isHidden | boolean | se il PivotItem specifico è nascosto |

### hideItem(String itemValue, boolean isHidden) {#hideItem-java.lang.String-boolean-}
```
public void hideItem(String itemValue, boolean isHidden)
```


Imposta se lo specifico PivotItem in un campo dati è nascosto.

**Remarks**

NOTE: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems[string].IsHidden. Questo metodo sarà rimosso tra 12 mesi a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| itemValue | java.lang.String | Il nome del pivotItem nel pivotField. |
| isHidden | boolean | Se il PivotItem specifico è nascosto |

### hideItemDetail(int index, boolean isHiddenDetail) {#hideItemDetail-int-boolean-}
```
public void hideItemDetail(int index, boolean isHiddenDetail)
```


Imposta se il dettaglio dello specifico PivotItem in un campo pivot è nascosto.

**Remarks**

NOTE: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems[int].IsDetailHidden. Questo metodo sarà rimosso tra 12 mesi a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | l'indice del pivotItem nel pivotField. |
| isHiddenDetail | boolean | se il PivotItem specifico è nascosto |

### initPivotItems() {#initPivotItems--}
```
public void initPivotItems()
```


Inizializza gli elementi pivot del campo pivot

**Remarks**

NOTE: Questo metodo è ora obsoleto. Si prega semplicemente di rimuovere la chiamata a questo metodo. Questo metodo sarà rimosso tra 6 mesi a partire da ottobre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

### isAscendShow() {#isAscendShow--}
```
public boolean isAscendShow()
```


Indica se il campo PivotTable specificato è mostrato automaticamente in ordine ascendente.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.IsTop o il metodo PivotField.Top10AutoShow(). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
boolean
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


Indica se gli elementi di questo campo pivot sono ordinati automaticamente in modo ascendente.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.SortSetting.SortType o il metodo PivotField.SortBy(). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Indica se il campo PivotTable specificato è mostrato automaticamente.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.IsAutoShow o il metodo PivotField.Top10AutoShow(). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


Indica se gli elementi di questo campo PivotTable sono ordinati automaticamente.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.SortSetting.SortType o il metodo PivotField.SortBy(). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
boolean
### isAutoSubtotals() {#isAutoSubtotals--}
```
public boolean isAutoSubtotals()
```


Indica se il campo specificato mostra subtotali automatici. Il valore predefinito è true.

**Returns:**
boolean
### isCalculatedField() {#isCalculatedField--}
```
public boolean isCalculatedField()
```


Indica se questo campo pivot è un campo calcolato.

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


Indica se lo specifico PivotItem è nascosto.

**Remarks**

NOTE: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems[int].IsHidden. Questo metodo sarà rimosso tra 12 mesi a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice del pivotItem nel pivotField. |

**Returns:**
booleano - se il PivotItem specifico è nascosto
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


Indica se nascondere il dettaglio dello specifico PivotItem..

**Remarks**

NOTE: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems[int].IsDetailHidden. Questo metodo sarà rimosso tra 12 mesi a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice del pivotItem nel pivotField. |

**Returns:**
booleano - se il dettaglio del PivotItem specifico è nascosto
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


Indica se includere nuovi elementi al campo nel filtro manuale. Il valore predefinito è false.

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


Indica se inserire interruzioni di pagina dopo ogni elemento. Il valore predefinito è false.

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


Indica se più elementi possono essere selezionati nel campo pagina. Il valore predefinito è false.

**Remarks**

Solo per i campi pagina (filtro).

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


Indica se ripetere le etichette del campo nella regione riga o colonna. Il valore predefinito è false.

**Returns:**
boolean
### isValueFields() {#isValueFields--}
```
public boolean isValueFields()
```


Indica se questo campo rappresenta campi valori.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.IsValuesField. Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
boolean
### isValuesField() {#isValuesField--}
```
public boolean isValuesField()
```


Indica se questo campo rappresenta un campo valore.

**Remarks**

Funziona solo quando ci sono due o più campi dati nella vista della tabella pivot.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllowDraggingToColumn(boolean value) {#setAllowDraggingToColumn-boolean-}
```
public void setAllowDraggingToColumn(boolean value)
```


Indica se il campo specificato può essere trascinato nella regione colonna. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowDraggingToData(boolean value) {#setAllowDraggingToData-boolean-}
```
public void setAllowDraggingToData(boolean value)
```


Indica se il campo specificato può essere trascinato nella regione valori. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowDraggingToPage(boolean value) {#setAllowDraggingToPage-boolean-}
```
public void setAllowDraggingToPage(boolean value)
```


Indica se il campo specificato può essere trascinato nella regione pagina. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowDraggingToRow(boolean value) {#setAllowDraggingToRow-boolean-}
```
public void setAllowDraggingToRow(boolean value)
```


Indica se il campo specificato può essere trascinato nella regione riga. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAllowRemovingFromView(boolean value) {#setAllowRemovingFromView-boolean-}
```
public void setAllowRemovingFromView(boolean value)
```


Indica se questo campo pivot può essere rimosso dalla visualizzazione della tabella pivot. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAscendShow(boolean value) {#setAscendShow-boolean-}
```
public void setAscendShow(boolean value)
```


Indica se il campo PivotTable specificato è mostrato automaticamente in ordine ascendente.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.IsTop o il metodo PivotField.Top10AutoShow(). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


Indica se gli elementi di questo campo pivot sono ordinati automaticamente in modo ascendente.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.SortSetting.SortType o il metodo PivotField.SortBy(). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Indica se il campo PivotTable specificato è mostrato automaticamente.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.IsAutoShow o il metodo PivotField.Top10AutoShow(). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Rappresenta il numero di elementi superiori o inferiori visualizzati automaticamente nel campo PivotTable specificato.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.AutoShowCount o il metodo PivotField.Top10AutoShow() . Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


Rappresenta l'indice del campo auto‑show. -1 indica il PivotField stesso. Deve essere l'indice dei campi dati.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.Top10AutoShowSettings.RankBy o il metodo PivotField.Top10AutoShow() . Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


Indica se gli elementi di questo campo PivotTable sono ordinati automaticamente.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.SortSetting.SortType o il metodo PivotField.SortBy(). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


Rappresenta l'indice del campo che è ordinato automaticamente. -1 indica il PivotField stesso, altri valori indicano la posizione dei campi dati.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.SortSetting.SortBy o il metodo PivotField.SortBy() . Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


Indica se il campo specificato mostra subtotali automatici. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


Rappresenta l'indice nei campi pivot di origine.

**Remarks**

NOTA: Questo setter di questa proprietà è ora obsoleto. Questo setter sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


Imposta l'elemento di pagina attualmente visualizzato per questo campo pivot (solo campo pagina).

**Remarks**

Utilizzare [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) come valore sentinella per indicare \"Select All\". Questo è un marcatore predefinito e non è un indice di elemento valido.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | short |  |

### setCurrentPageItemText(String value) {#setCurrentPageItemText-java.lang.String-}
```
public void setCurrentPageItemText(String value)
```


Ottiene il testo visualizzato dell'elemento di pagina corrente per questo campo pivot (solo campo pagina).

**Remarks**

Restituisce \"(All)\" quando [getCurrentPageItem()](../../com.aspose.cells/pivotfield\\#getCurrentPageItem--) è uguale a [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX). Per altri valori, restituisce la rappresentazione stringa dell'indice dell'elemento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Rappresenta il nome visualizzato del campo pivot nella visualizzazione della tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


Indica se il campo specificato può essere trascinato nella regione colonna. Il valore predefinito è true.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToColumn. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


Indica se il campo specificato può essere trascinato nella regione valori. Il valore predefinito è true.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToData. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


Indica se questo campo pivot può essere rimosso dalla visualizzazione della tabella pivot. Il valore predefinito è true.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowRemovingFromView. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


Indica se il campo specificato può essere trascinato nella regione pagina. Il valore predefinito è true.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToPage. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


Indica se il campo specificato può essere trascinato nella regione riga. Il valore predefinito è true.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.AllowDraggingToRow. Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


Rappresenta la funzione utilizzata per riepilogare questo campo dati della PivotTable.

Vedi [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


Indica se includere nuovi elementi al campo nel filtro manuale. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


Indica se inserire una riga vuota dopo ogni elemento. Solo per i campi di riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


Indica se inserire interruzioni di pagina dopo ogni elemento. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


Indica se più elementi possono essere selezionati nel campo pagina. Il valore predefinito è false.

**Remarks**

Solo per i campi pagina (filtro).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Rappresenta il nome di PivotField.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


Indica se un'operazione di ordinamento che verrà applicata a questo campo pivot è un'operazione di autosort o un semplice ordinamento dei dati.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà !PivotField.SortSetting.IsSimpleSort. Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Rappresenta il formato di visualizzazione integrato di numeri e date.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Rappresenta il formato di visualizzazione personalizzato di numeri e date.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


Indica se ripetere le etichette del campo nella regione riga o colonna. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Indica se visualizzare tutti gli elementi nella vista PivotTable, anche se non contengono dati di riepilogo. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


Indica se visualizzare le etichette del campo successivo nella stessa colonna nella vista Pivot Table. Solo per i campi di riga.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.ShowInCompactForm. Questo metodo sarà rimosso 12 mesi dopo a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowInCompactForm(boolean value) {#setShowInCompactForm-boolean-}
```
public void setShowInCompactForm(boolean value)
```


Imposta un valore che indica se questo campo riga utilizza il layout a forma compatta. Si applica solo ai campi riga.

**Remarks**

La forma compatta è una sotto-modalità del layout a contorno. Questa impostazione ha effetto solo quando [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


Imposta un valore che indica se questo campo riga utilizza il layout a contorno. Si applica solo ai campi riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


Indica se visualizzare i subtotali in cima o in fondo agli elementi.

**Remarks**

Funziona solo per i campi pivot nella regione di riga quando ShowInOutlineForm è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSubtotals(int value) {#setSubtotals-int-}
```
public void setSubtotals(int value)
```


Imposta i subtotali del campo. Solo per i campi Pivot di tipo Riga o Colonna.

Vedi [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Imposta come subtotale il campo specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| mostrato | boolean | Indica se il campo specificato mostra quei subtotali. |

### showAllDetails() {#showAllDetails--}
```
public void showAllDetails()
```


Mostra tutti i dettagli di ciascun elemento pivot.

### showValuesAs(int showValuesAsType, int baseField, int baseItem) {#showValuesAs-int-int-int-}
```
public void showValuesAs(int showValuesAsType, int baseField, int baseItem)
```


Imposta il calcolo "Mostra valori come" per questo campo pivot.

**Remarks**

Solo per il campo dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Tipo del calcolo \"Show Values As\". |
| baseField | int | Indice del campo base utilizzato per il calcolo. |
| baseItem | int | Indice dell'elemento base per il calcolo. Utilizzare [PivotShowValuesSetting.PREVIOUS\\_PIVOT\\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\\#PREVIOUS-PIVOT-ITEM) (-1) per l'elemento precedente, [PivotShowValuesSetting.NEXT\\_PIVOT\\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\\#NEXT-PIVOT-ITEM) (-2) per l'elemento successivo; valori non\\\\u9225\\\\u6182egativi indicano l'indice ordinale di un elemento pivot specifico. |

### showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem) {#showValuesAs-int-int-int-int-}
```
public void showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)
```


Mostra i valori del campo dati in un formato di visualizzazione diverso quando è in uso il calcolo ShowDataAs.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| displayFormat | int | [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat). Il tipo di formato di visualizzazione dei dati. |
| baseField | int | L'indice del campo su cui si basa il calcolo ShowDataAs. |
| baseItemPositionType | int | [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype). Il tipo di posizione dell'elemento base. |
| baseItem | int | L'indice dell'elemento base su cui si basa il calcolo ShowDataAs. Funziona solo quando baseItemPositionType è personalizzato. |

### showValuesAs(int showValuesAsType, String baseField, String baseItem) {#showValuesAs-int-java.lang.String-java.lang.String-}
```
public void showValuesAs(int showValuesAsType, String baseField, String baseItem)
```


Configura il calcolo "Mostra valori come" per questo campo dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Il tipo di calcolo per Show Values As. |
| baseField | java.lang.String | Il nome del campo base utilizzato nel calcolo. |
| baseItem | java.lang.String | Didascalia di un elemento pivot regolare. Accetta anche parole chiave letterali riservate: `(previous)` per l'elemento precedente, `(next)` per l'elemento successivo. Passare `null` se il tipo di calcolo selezionato non richiede un elemento base. |

### sortBy(int sortType) {#sortBy-int-}
```
public void sortBy(int sortType)
```


Ordina questo campo pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Il tipo di ordinamento di questo campo. |

### sortBy(int sortType, int fieldSortedBy) {#sortBy-int-int-}
```
public void sortBy(int sortType, int fieldSortedBy)
```


Ordina questo campo pivot.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotField.SortBy(SortOrder, int,string) o la proprietà PivotField.IsAutoSort. Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Il tipo di ordinamento di questo campo. |
| fieldSortedBy | int | L'indice del campo pivot per cui è ordinato. -1 indica l'ordinamento per le etichette dati di questo campo, altri valori indicano l'indice del campo dati per cui è ordinato. |

### sortBy(int sortType, int fieldSortedBy, int dataType, String cellName) {#sortBy-int-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)
```


Ordina questo campo pivot.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotField.SortBy(SortOrder, int,string). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Il tipo di ordinamento di questo campo. |
| fieldSortedBy | int | L'indice del campo pivot per cui è ordinato. -1 indica l'ordinamento per le etichette dati di questo campo, altri valori indicano l'indice del campo dati per cui è ordinato. |
| dataType | int | [PivotLineType](../../com.aspose.cells/pivotlinetype). Il tipo di dati per cui è ordinato. |
| cellName | java.lang.String | Ordina per valori nella riga o nella colonna |

### sortBy(int sortType, int fieldSortedBy, String cellName) {#sortBy-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, String cellName)
```


Ordina questo campo pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Il tipo di ordinamento di questo campo. |
| fieldSortedBy | int | L'indice del campo pivot per cui è ordinato. -1 indica l'ordinamento per le etichette dati di questo campo, altri valori indicano l'indice del campo dati per cui è ordinato. |
| cellName | java.lang.String | Ordina per valori nella riga o nella colonna. Se Null, raggruppa per il totale del campo, altrimenti raggruppa per i valori nella colonna o riga selezionata. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy) {#top10AutoShow-boolean-boolean-int-int-}
```
public void top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)
```


Configura le impostazioni Top10 AutoShow per questo campo pivot.

**Remarks**

Questo metodo configura il formato binario .XLS: AutoShow (Top10) è l'opzione nativa e l'unica supportata. XLSX (OpenXML): il formato di file sottostante supporta Top10 AutoShow, ma l'interfaccia utente di Excel 2007 e successive lo espone solo tramite il filtro Top10. Se la compatibilità XLS non è necessaria, si consiglia di utilizzare invece il filtro Top10.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isAutoShow | boolean | true per abilitare AutoShow; false per disabilitarlo. |
| isTop | boolean | Se true, mostra gli elementi superiori; false mostra gli elementi inferiori. |
| count | int | Numero di elementi superiori/inferiori da visualizzare. |
| rankBy | int | Indice del campo dati utilizzato per il ranking. Usare -1 per classificare in base ai valori propri dell'elemento pivot. |

### ungroup() {#ungroup--}
```
public void ungroup()
```


Annulla il raggruppamento del campo pivot.

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

