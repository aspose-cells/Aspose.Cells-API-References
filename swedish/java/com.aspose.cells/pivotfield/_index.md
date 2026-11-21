---
title: "PivotField"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett fält i en pivottabellsrapport."
type: docs
url: /sv/java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

Representerar ett fält i en pivottabellsrapport.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | Lägg till ett beräknat formelobjekt till pivotfältet. |
| [clearFilter()](#clearFilter--) | Rensar filterinställningarna på detta pivotfält. |
| [dispose()](#dispose--) | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterByDate(int type, DateTime dateTime1, DateTime dateTime2)](#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filtrerar efter datumvärden för rad- eller kolumnpivotfält. |
| [filterByLabel(int type, String label1, String label2)](#filterByLabel-int-java.lang.String-java.lang.String-) | Filtrerar efter rubriker för rad- eller kolumnpivotfält. |
| [filterByValue(int valueFieldIndex, int type, double value1, double value2)](#filterByValue-int-int-double-double-) | Filtrerar efter värden för datapivotfält. |
| [filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)](#filterTop10-int-int-boolean-int-) | Filtrerar efter värden för datapivotfält. |
| [getAllowDraggingToColumn()](#getAllowDraggingToColumn--) | Anger om det specificerade fältet kan dras till kolumnregionen. |
| [getAllowDraggingToData()](#getAllowDraggingToData--) | Anger om det specificerade fältet kan dras till värdeområdet. |
| [getAllowDraggingToPage()](#getAllowDraggingToPage--) | Anger om det specificerade fältet kan dras till sidregionen. |
| [getAllowDraggingToRow()](#getAllowDraggingToRow--) | Anger om det specificerade fältet kan dras till radregionen. |
| [getAllowRemovingFromView()](#getAllowRemovingFromView--) | Anger om detta pivotfält kan tas bort från PivotTable-vyn. |
| [getAutoShowCount()](#getAutoShowCount--) | Representerar antalet översta eller nedersta objekt som automatiskt visas i det angivna PivotTable-fältet. |
| [getAutoShowField()](#getAutoShowField--) | Representerar index för automatiskt visat fält. -1 betyder PivotField själv. |
| [getAutoSortField()](#getAutoSortField--) | Representerar index för fält som sorteras automatiskt. |
| [getBaseIndex()](#getBaseIndex--) | Representerar indexet i källpivotfälten. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | Hämta formelsträngen för det angivna beräknade fältet . |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | Hämtar det för närvarande visade sidobjektet för detta pivottfält (endast sidfält). |
| [getCurrentPageItemText()](#getCurrentPageItemText--) | Hämtar visningstexten för det aktuella sidobjektet för detta pivottfält (endast sidfält). |
| [getDisplayName()](#getDisplayName--) | Representerar visningsnamnet för pivottfältet i pivottabellvyn. |
| [getDragToColumn()](#getDragToColumn--) | Anger om det specificerade fältet kan dras till kolumnregionen. |
| [getDragToData()](#getDragToData--) | Anger om det specificerade fältet kan dras till värdeområdet. |
| [getDragToHide()](#getDragToHide--) | Anger om detta pivotfält kan tas bort från PivotTable-vyn. |
| [getDragToPage()](#getDragToPage--) | Anger om det specificerade fältet kan dras till sidregionen. |
| [getDragToRow()](#getDragToRow--) | Anger om det specificerade fältet kan dras till radregionen. |
| [getFilters()](#getFilters--) | Hämtar alla pivottfilter som tillämpas för detta pivottfält. |
| [getFormula()](#getFormula--) | Hämtar formeln för det beräknade fältet . |
| [getFunction()](#getFunction--) | Representerar funktionen som används för att sammanfatta detta PivotTable-datafält. |
| [getGroupSettings()](#getGroupSettings--) | Hämtar grupperingens inställningar för pivottfältet. |
| [getInsertBlankRow()](#getInsertBlankRow--) | Anger om en tom rad ska infogas efter varje objekt. |
| [getItemCount()](#getItemCount--) | Hämtar antalet basobjekt i detta pivottfält. |
| [getItems()](#getItems--) | Hämta alla etiketter för pivottobjekt i detta fält. |
| [getMaxValue()](#getMaxValue--) | Hämtar det maximala värdet för detta fält. |
| [getMinValue()](#getMinValue--) | Hämtar det maximala värdet för detta fält. |
| [getName()](#getName--) | Representerar namnet på PivotField. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | Anger om en sorteringsoperation som kommer att tillämpas på detta pivottfält är en autosortering eller en enkel datasortering. |
| [getNumber()](#getNumber--) | Representerar det inbyggda visningsformatet för tal och datum. |
| [getNumberFormat()](#getNumberFormat--) | Representerar det anpassade visningsformatet för tal och datum. |
| [getOriginalItems()](#getOriginalItems--) | Hämta de ursprungliga basobjekten; |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | Hämtar pivottfiltret för pivottfältet efter typ |
| [getPivotFilters()](#getPivotFilters--) | Hämtar pivottfiltren för pivottfältet |
| [getPivotItems()](#getPivotItems--) | Hämtar pivottobjekten för pivottfältet |
| [getPosition()](#getPosition--) | Representerar indexet för [PivotField](../../com.aspose.cells/pivotfield) i regionen. |
| [getRegionType()](#getRegionType--) | Anger regionen för pivottabellen där detta fält visas. |
| [getShowAllItems()](#getShowAllItems--) | Anger om alla objekt ska visas i PivotTable-vyn, även om de inte innehåller sammanfattningsdata. |
| [getShowCompact()](#getShowCompact--) | Anger om etiketter för nästa fält i samma kolumn ska visas i Pivot Table-vyn. |
| [getShowInCompactForm()](#getShowInCompactForm--) | Hämtar ett värde som indikerar om detta radfält använder kompakt form-layout. |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | Hämtar ett värde som indikerar om detta radfält använder konturlayout. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | Anger om delsummer ska visas högst upp eller längst ner på objekten. |
| [getShowValuesSetting()](#getShowValuesSetting--) | Hämtar inställningarna för att visa värden som när beräkningen ShowDataAs används. |
| [getSortSetting()](#getSortSetting--) | Hämtar alla inställningar för automatisk sortering. |
| [getSubtotals()](#getSubtotals--) | Hämtar fältets delsummer. |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | Anger om angiven delsumma ska visas för detta pivåtfält. |
| [getTop10AutoShowSettings()](#getTop10AutoShowSettings--) | Hämtar Top 10 AutoShow-inställningarna för ett pivåtfält. |
| [group()](#group--) | Gruppera fältet automatiskt. |
| [group(PivotFieldGroupOptions options)](#group-com.aspose.cells.PivotFieldGroupOptions-) | Grupperar pivåtfältet med alternativ. |
| [groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-) | Gruppera filen efter datumgruppstyper. |
| [groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)](#groupBy-boolean-double-boolean-double-double-boolean-) | Gruppera filen efter nummer. |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | Anpassa gruppering av fältet. |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | Gruppera filen efter datumgruppstyper. |
| [groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-) | Anpassa gruppering av fältet. |
| [groupBy(double interval, boolean newField)](#groupBy-double-boolean-) | Gruppera fältet automatiskt med intervall. |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | Gruppera filen efter nummer. |
| [groupBy(int[] groups, double interval, boolean newField)](#groupBy-int---double-boolean-) | Gruppera fältet automatiskt internt. |
| [hashCode()](#hashCode--) |  |
| [hideAllDetails()](#hideAllDetails--) | Döljer alla detaljer för varje pivåtelement. |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | Ställer in om detaljen för alla PivotItems i ett pivåtfält är dold. |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | Ställer in om det specifika PivotItem i ett datafält är dolt. |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | Ställer in om det specifika PivotItem i ett datafält är dolt. |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | Ställer in om den specifika PivotItem i ett pivåtfält har dold detalj. |
| [initPivotItems()](#initPivotItems--) | Initiera pivåtelementen för pivåtfältet. |
| [isAscendShow()](#isAscendShow--) | Indikerar om det angivna PivotTable-fältet automatiskt visas i stigande ordning. |
| [isAscendSort()](#isAscendSort--) | Anger om objekten i detta pivåtfält är automatiskt sorterade stigande. |
| [isAutoShow()](#isAutoShow--) | Anger om det angivna PivotTable-fältet visas automatiskt. |
| [isAutoSort()](#isAutoSort--) | Anger om objekten i detta PivotTable-fält är automatiskt sorterade. |
| [isAutoSubtotals()](#isAutoSubtotals--) | Anger om det angivna fältet visar automatiska delsummer. |
| [isCalculatedField()](#isCalculatedField--) | Anger om detta pivåtfält är ett beräknat fält. |
| [isHiddenItem(int index)](#isHiddenItem-int-) | Anger om det specifika PivotItem är dolt. |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | Anger om detaljen för det specifika PivotItem ska döljas.. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | Anger om nya objekt ska inkluderas i fältet i manuellt filter. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | Anger om sidbrytningar ska infogas efter varje objekt. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | Anger om flera objekt kan väljas i sidfältet. |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | Anger om etiketter för fältet ska upprepas i rad- eller kolumnområdet. |
| [isValueFields()](#isValueFields--) | Anger om detta fält representerar värdefält. |
| [isValuesField()](#isValuesField--) | Anger om detta fält representerar värdefält. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDraggingToColumn(boolean value)](#setAllowDraggingToColumn-boolean-) | Anger om det specificerade fältet kan dras till kolumnregionen. |
| [setAllowDraggingToData(boolean value)](#setAllowDraggingToData-boolean-) | Anger om det specificerade fältet kan dras till värdeområdet. |
| [setAllowDraggingToPage(boolean value)](#setAllowDraggingToPage-boolean-) | Anger om det specificerade fältet kan dras till sidregionen. |
| [setAllowDraggingToRow(boolean value)](#setAllowDraggingToRow-boolean-) | Anger om det specificerade fältet kan dras till radregionen. |
| [setAllowRemovingFromView(boolean value)](#setAllowRemovingFromView-boolean-) | Anger om detta pivotfält kan tas bort från PivotTable-vyn. |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | Indikerar om det angivna PivotTable-fältet automatiskt visas i stigande ordning. |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Anger om objekten i detta pivåtfält är automatiskt sorterade stigande. |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Anger om det angivna PivotTable-fältet visas automatiskt. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Representerar antalet översta eller nedersta objekt som automatiskt visas i det angivna PivotTable-fältet. |
| [setAutoShowField(int value)](#setAutoShowField-int-) | Representerar index för automatiskt visat fält. -1 betyder PivotField själv. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Anger om objekten i detta PivotTable-fält är automatiskt sorterade. |
| [setAutoSortField(int value)](#setAutoSortField-int-) | Representerar index för fält som sorteras automatiskt. |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | Anger om det angivna fältet visar automatiska delsummer. |
| [setBaseIndex(int value)](#setBaseIndex-int-) | Representerar indexet i källpivotfälten. |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | Ställer in det för närvarande visade sidobjektet för detta pivåtfält (endast sidfält). |
| [setCurrentPageItemText(String value)](#setCurrentPageItemText-java.lang.String-) | Hämtar visningstexten för det aktuella sidobjektet för detta pivottfält (endast sidfält). |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Representerar visningsnamnet för pivottfältet i pivottabellvyn. |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | Anger om det specificerade fältet kan dras till kolumnregionen. |
| [setDragToData(boolean value)](#setDragToData-boolean-) | Anger om det specificerade fältet kan dras till värdeområdet. |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | Anger om detta pivotfält kan tas bort från PivotTable-vyn. |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | Anger om det specificerade fältet kan dras till sidregionen. |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | Anger om det specificerade fältet kan dras till radregionen. |
| [setFunction(int value)](#setFunction-int-) | Representerar funktionen som används för att sammanfatta detta PivotTable-datafält. |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | Anger om nya objekt ska inkluderas i fältet i manuellt filter. |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | Anger om en tom rad ska infogas efter varje objekt. |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | Anger om sidbrytningar ska infogas efter varje objekt. |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | Anger om flera objekt kan väljas i sidfältet. |
| [setName(String value)](#setName-java.lang.String-) | Representerar namnet på PivotField. |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | Anger om en sorteringsoperation som kommer att tillämpas på detta pivottfält är en autosortering eller en enkel datasortering. |
| [setNumber(int value)](#setNumber-int-) | Representerar det inbyggda visningsformatet för tal och datum. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Representerar det anpassade visningsformatet för tal och datum. |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | Anger om etiketter för fältet ska upprepas i rad- eller kolumnområdet. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Anger om alla objekt ska visas i PivotTable-vyn, även om de inte innehåller sammanfattningsdata. |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | Anger om etiketter för nästa fält i samma kolumn ska visas i Pivot Table-vyn. |
| [setShowInCompactForm(boolean value)](#setShowInCompactForm-boolean-) | Ställer in ett värde som anger om detta radfält använder kompakt formlayout. |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | Ställer in ett värde som anger om detta radfält använder konturlayout. |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | Anger om delsummer ska visas högst upp eller längst ner på objekten. |
| [setSubtotals(int value)](#setSubtotals-int-) | Ställer in delsummerna för fältet. |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Ställer in hur det angivna fältet ska delsummeras. |
| [showAllDetails()](#showAllDetails--) | Visa alla detaljer för varje pivåtelement. |
| [showValuesAs(int showValuesAsType, int baseField, int baseItem)](#showValuesAs-int-int-int-) | Ställer in beräkningen "Show Values As" för detta pivåtfält. |
| [showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)](#showValuesAs-int-int-int-int-) | Visar värden för datafältet i annat displayformat när beräkningen ShowDataAs används. |
| [showValuesAs(int showValuesAsType, String baseField, String baseItem)](#showValuesAs-int-java.lang.String-java.lang.String-) | Konfigurerar beräkningen "Show Values As" för detta datafält. |
| [sortBy(int sortType)](#sortBy-int-) | Sorterar detta pivåtfält. |
| [sortBy(int sortType, int fieldSortedBy)](#sortBy-int-int-) | Sorterar detta pivåtfält. |
| [sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)](#sortBy-int-int-int-java.lang.String-) | Sorterar detta pivåtfält. |
| [sortBy(int sortType, int fieldSortedBy, String cellName)](#sortBy-int-int-java.lang.String-) | Sorterar detta pivåtfält. |
| [toString()](#toString--) |  |
| [top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)](#top10AutoShow-boolean-boolean-int-int-) | Konfigurerar Top10 AutoShow-inställningarna för detta pivåtfält. |
| [ungroup()](#ungroup--) | Avgruppera pivåtfältet. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


Lägg till ett beräknat formelobjekt till pivotfältet.

**Remarks**

Stöder endast att lägga till beräknat objekt till rad-/kolumnfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Objektets namn. |
| formula | java.lang.String | Formeln för pivåtelementet. |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Rensar filterinställningarna på detta pivotfält.

### dispose() {#dispose--}
```
public void dispose()
```


Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### filterByDate(int type, DateTime dateTime1, DateTime dateTime2) {#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter filterByDate(int type, DateTime dateTime1, DateTime dateTime2)
```


Filtrerar efter datumvärden för rad- eller kolumnpivotfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Typen av filtreringsdata. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | Datumetiketten för filtervillkoret |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | Den övre gränsens datumetikett för mellanfiltervillkoret |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByLabel(int type, String label1, String label2) {#filterByLabel-int-java.lang.String-java.lang.String-}
```
public PivotFilter filterByLabel(int type, String label1, String label2)
```


Filtrerar efter rubriker för rad- eller kolumnpivotfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Typen av filtreringsdata. |
| label1 | java.lang.String | Etiketten för filtervillkoret |
| label2 | java.lang.String | Den övre gränsens etikett för mellanfiltervillkoret |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByValue(int valueFieldIndex, int type, double value1, double value2) {#filterByValue-int-int-double-double-}
```
public PivotFilter filterByValue(int valueFieldIndex, int type, double value1, double value2)
```


Filtrerar efter värden för datapivotfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| valueFieldIndex | int | Index för värdefältet i värdeområdet. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Typen av filtreringsdata. |
| value1 | double | Värdet för filtervillkoret. |
| value2 | double | Det övre gränsvärdet för mellanfiltervillkoret. |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount) {#filterTop10-int-int-boolean-int-}
```
public PivotFilter filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filtrerar efter värden för datapivotfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| valueFieldIndex | int | Index för datafältet i dataområdet. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Typ av filtreringsdata. Kan endast vara Count, Sum och Percent. |
| isTop | boolean | Indikerar om filtret är från toppen eller botten. |
| itemCount | int | Antalet objekt. |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getAllowDraggingToColumn() {#getAllowDraggingToColumn--}
```
public boolean getAllowDraggingToColumn()
```


Anger om det angivna fältet kan dras till kolumnområdet. Standardvärdet är sant.

**Returns:**
boolean
### getAllowDraggingToData() {#getAllowDraggingToData--}
```
public boolean getAllowDraggingToData()
```


Anger om det angivna fältet kan dras till värdeområdet. Standardvärdet är sant.

**Returns:**
boolean
### getAllowDraggingToPage() {#getAllowDraggingToPage--}
```
public boolean getAllowDraggingToPage()
```


Anger om det angivna fältet kan dras till sidområdet. Standardvärdet är sant.

**Returns:**
boolean
### getAllowDraggingToRow() {#getAllowDraggingToRow--}
```
public boolean getAllowDraggingToRow()
```


Anger om det angivna fältet kan dras till radregionen. Standardvärdet är sant.

**Returns:**
boolean
### getAllowRemovingFromView() {#getAllowRemovingFromView--}
```
public boolean getAllowRemovingFromView()
```


Anger om detta pivottfält kan tas bort från PivotTable-vyn. Standardvärdet är sant.

**Returns:**
boolean
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Representerar antalet översta eller nedersta objekt som automatiskt visas i det angivna PivotTable-fältet.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.Top10AutoShowSettings.AutoShowCount eller metoden PivotField.Top10AutoShow() istället. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getAutoShowField() {#getAutoShowField--}
```
public int getAutoShowField()
```


Representerar index för automatisk visning av fält. -1 betyder PivotField själv. Det bör vara indexet för datafälten.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.Top10AutoShowSettings.RankBy eller metoden PivotField.Top10AutoShow() istället. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getAutoSortField() {#getAutoSortField--}
```
public int getAutoSortField()
```


Representerar indexet för fältet som sorteras automatiskt. -1 betyder PivotField själv, andra betyder positionen för datafälten.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.SortSetting.SortBy eller metoden PivotField.SortBy() istället. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


Representerar indexet i källpivotfälten.

**Remarks**

OBS: Denna setter för egenskapen är nu föråldrad. Denna setter för egenskapen kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


Hämta formelsträngen för det angivna beräknade fältet .

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden PivotField.GetFormula(). Denna metod kommer att tas bort 12 månader senare från och med augusti 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Hämtar det för närvarande visade sidobjektet för detta pivottfält (endast sidfält).

**Remarks**

Använd [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) som sentinelvärde för att indikera \"Select All\". Detta är en fördefinierad markör och är inte ett giltigt objektindex.

**Returns:**
short
### getCurrentPageItemText() {#getCurrentPageItemText--}
```
public String getCurrentPageItemText()
```


Hämtar visningstexten för det aktuella sidobjektet för detta pivottfält (endast sidfält).

**Remarks**

Returnerar \"(All)\" när [getCurrentPageItem()](../../com.aspose.cells/pivotfield\\#getCurrentPageItem--) är lika med [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX). För andra värden returneras strängrepresentationen av objektindexet.

**Returns:**
java.lang.String
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Representerar visningsnamnet för pivottfältet i pivottabellvyn.

**Returns:**
java.lang.String
### getDragToColumn() {#getDragToColumn--}
```
public boolean getDragToColumn()
```


Anger om det angivna fältet kan dras till kolumnområdet. Standardvärdet är sant.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.AllowDraggingToColumn. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getDragToData() {#getDragToData--}
```
public boolean getDragToData()
```


Anger om det angivna fältet kan dras till värdeområdet. Standardvärdet är sant.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.AllowDraggingToData. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


Anger om detta pivottfält kan tas bort från PivotTable-vyn. Standardvärdet är sant.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.AllowRemovingFromView. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getDragToPage() {#getDragToPage--}
```
public boolean getDragToPage()
```


Anger om det angivna fältet kan dras till sidområdet. Standardvärdet är sant.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.AllowDraggingToPage. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getDragToRow() {#getDragToRow--}
```
public boolean getDragToRow()
```


Anger om det angivna fältet kan dras till radregionen. Standardvärdet är sant.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.AllowDraggingToRow. Denna metod kommer att tas bort 12 månader senare, från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getFilters() {#getFilters--}
```
public PivotFilter[] getFilters()
```


Hämtar alla pivottfilter som tillämpas för detta pivottfält.

**Returns:**
com.aspose.cells.PivotFilter[]
### getFormula() {#getFormula--}
```
public String getFormula()
```


Hämtar formeln för det beräknade fältet. Fungerar endast för det beräknade fältet.

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


Representerar funktionen som används för att sammanfatta detta PivotTable-datafält.

Se [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


Hämtar grupperingens inställningar för pivottfältet.

**Remarks**

Om detta fält inte är grupperat returneras Null.

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


Anger om en tom rad ska infogas efter varje objekt. Endast för radfält.

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


Hämtar antalet basobjekt i detta pivottfält.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället egenskapen PivotField.PivotItems.Count. Denna metod kommer att tas bort 12 månader senare, från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


Hämta alla etiketter för pivottobjekt i detta fält.

**Returns:**
java.lang.String[]
### getMaxValue() {#getMaxValue--}
```
public CellValue getMaxValue()
```


Hämtar det maximala värdet för detta fält.

**Remarks**

Fungerar endast för rad- eller kolumnfält vars värde måste vara datum/tid, tal eller tomt.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getMinValue() {#getMinValue--}
```
public CellValue getMinValue()
```


Hämtar det maximala värdet för detta fält.

**Remarks**

Fungerar endast för rad- eller kolumnfält vars värde måste vara datum/tid, tal eller tomt.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getName() {#getName--}
```
public String getName()
```


Representerar namnet på PivotField.

**Returns:**
java.lang.String
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```
public boolean getNonAutoSortDefault()
```


Anger om en sorteringsoperation som kommer att tillämpas på detta pivottfält är en autosortering eller en enkel datasortering.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen !PivotField.SortSetting.IsSimpleSort. Denna metod kommer att tas bort 12 månader senare, från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getNumber() {#getNumber--}
```
public int getNumber()
```


Representerar det inbyggda visningsformatet för tal och datum.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Representerar det anpassade visningsformatet för tal och datum.

**Returns:**
java.lang.String
### getOriginalItems() {#getOriginalItems--}
```
public String[] getOriginalItems()
```


Hämta de ursprungliga basobjekten;

**Returns:**
java.lang.String[]
### getPivotFilterByType(int type) {#getPivotFilterByType-int-}
```
public PivotFilter getPivotFilterByType(int type)
```


Hämtar pivottfiltret för pivottfältet efter typ

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getPivotFilters() {#getPivotFilters--}
```
public ArrayList getPivotFilters()
```


Hämtar pivottfiltren för pivottfältet

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden PivotField.GetFilters(). Denna metod kommer att tas bort 12 månader senare, från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.util.ArrayList
### getPivotItems() {#getPivotItems--}
```
public PivotItemCollection getPivotItems()
```


Hämtar pivottobjekten för pivottfältet

**Returns:**
[PivotItemCollection](../../com.aspose.cells/pivotitemcollection)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Representerar indexet för [PivotField](../../com.aspose.cells/pivotfield) i regionen.

**Returns:**
int
### getRegionType() {#getRegionType--}
```
public int getRegionType()
```


Anger regionen för pivottabellen där detta fält visas.

Se [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Anger om alla objekt ska visas i PivotTable-vyn, även om de inte innehåller sammanfattningsdata. Standardvärdet är false.

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


Anger om etiketter för nästa fält ska visas i samma kolumn i Pivot Table-vyn. Endast för radfält.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället egenskapen PivotField.ShowInCompactForm. Denna metod kommer att tas bort 12 månader senare, från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getShowInCompactForm() {#getShowInCompactForm--}
```
public boolean getShowInCompactForm()
```


Hämtar ett värde som anger om detta radfält använder kompakt form-layout. Gäller endast radfält.

**Remarks**

Kompakt form är ett delläge av kontur-layout. Denna inställning har bara effekt när [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) är true.

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


Hämtar ett värde som anger om detta radfält använder kontur-layout. Gäller endast radfält.

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


Anger om delsummer ska visas högst upp eller längst ner på objekten.

**Remarks**

Fungerar endast för pivåtfält i radregionen när ShowInOutlineForm är true.

**Returns:**
boolean
### getShowValuesSetting() {#getShowValuesSetting--}
```
public PivotShowValuesSetting getShowValuesSetting()
```


Hämtar inställningarna för att visa värden som när beräkningen ShowDataAs används.

**Returns:**
[PivotShowValuesSetting](../../com.aspose.cells/pivotshowvaluessetting)
### getSortSetting() {#getSortSetting--}
```
public PivotFieldSortSetting getSortSetting()
```


Hämtar alla inställningar för automatisk sortering.

**Returns:**
[PivotFieldSortSetting](../../com.aspose.cells/pivotfieldsortsetting)
### getSubtotals() {#getSubtotals--}
```
public int getSubtotals()
```


Hämtar delsummerna för fältet. Endast för rad- eller kolumn-pivåtfält.

Se [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

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


Anger om angiven delsumma ska visas för detta pivåtfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Subtotal-typ. |

**Returns:**
boolean - Returnerar om angiven delsumma visas.
### getTop10AutoShowSettings() {#getTop10AutoShowSettings--}
```
public PivotFieldTop10AutoShowSettings getTop10AutoShowSettings()
```


Hämtar Top 10 AutoShow-inställningarna för ett pivåtfält.

**Returns:**
[PivotFieldTop10AutoShowSettings](../../com.aspose.cells/pivotfieldtop10autoshowsettings)
### group() {#group--}
```
public boolean group()
```


Gruppera fältet automatiskt.

**Remarks**

Om fältet endast innehåller tomt och datum/tid, kommer fältet att grupperas efter månader. Om fältet endast innehåller tomt och tal, kommer fältet att grupperas efter tal. Annars returneras endast false utan någon gruppering.

**Returns:**
boolean
### group(PivotFieldGroupOptions options) {#group-com.aspose.cells.PivotFieldGroupOptions-}
```
public boolean group(PivotFieldGroupOptions options)
```


Grupperar pivåtfältet med alternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [PivotFieldGroupOptions](../../com.aspose.cells/pivotfieldgroupoptions) | Alternativ för gruppering av pivotfält. |

**Returns:**
boolean -
### groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Gruppera filen efter datumgruppstyper.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden PivotField.Group(PivotFieldGroupOptions). Denna metod kommer att tas bort 6 månader senare, från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAutoStart | boolean | Anger om startdatum/tid-värdet ska upptäckas automatiskt. |
| start | [DateTime](../../com.aspose.cells/datetime) | Startdatum och tid |
| isAutoEnd | boolean | Indikerar om slutdatum och tid ska upptäckas automatiskt. |
| end | [DateTime](../../com.aspose.cells/datetime) | Slutet av datum och tid |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Grupptyper |
| intervall | double | Intervallet |
| firstAsNewField | boolean | Indikerar om ett nytt fält ska läggas till i pivottabellen. Endast för det första grupperingselementet. |

**Returns:**
boolean - False betyder att detta fält inte kan grupperas efter datum och tid.
### groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField) {#groupBy-boolean-double-boolean-double-double-boolean-}
```
public boolean groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)
```


Gruppera filen efter nummer.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden PivotField.Group(PivotFieldGroupOptions). Denna metod kommer att tas bort 6 månader senare, från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAutoStart | boolean | Indikerar om startvärdet ska upptäckas automatiskt. |
| start | double | Startvärdet |
| isAutoEnd | boolean | Indikerar om slutvärdet ska upptäckas automatiskt. |
| end | double | Slutvärdet |
| intervall | double | Intervallet |
| newField | boolean | Indikerar om ett nytt fält ska läggas till i pivottabellen |

**Returns:**
boolean - False betyder att detta fält inte kan grupperas efter datum och tid.
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public boolean groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


Anpassa gruppering av fältet.

**Remarks**

OBS: Den här metoden är nu föråldrad. Använd istället metoden PivotField.Group(PivotFieldGroupOptions options) med egenskapen **PivotFieldGroupOptions.DiscreteGroupItems**. Denna metod kommer att tas bort 6 månader senare, från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | De anpassade gruppobjekten. |
| newField | boolean | Indikerar om ett nytt fält ska läggas till i pivottabellen |

**Returns:**
boolean - False betyder att detta fält inte kan grupperas efter datum och tid.
### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Gruppera filen efter datumgruppstyper.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden PivotField.Group(PivotFieldGroupOptions). Denna metod kommer att tas bort 6 månader senare, från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | Startdatum och tid |
| end | [DateTime](../../com.aspose.cells/datetime) | Slutet av datum och tid |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Grupptyper |
| intervall | double | Intervallet |
| firstAsNewField | boolean | Indikerar om ett nytt fält ska läggas till i pivottabellen. Endast för det första grupperingselementet. |

**Returns:**
boolean - False betyder att detta fält inte kan grupperas efter datum och tid.
### groupBy(DiscreteGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-}
```
public boolean groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)
```


Anpassa gruppering av fältet.

**Remarks**

OBS: Den här metoden är nu föråldrad. Använd istället metoden PivotField.Group(PivotFieldGroupOptions options) med egenskapen **PivotFieldGroupOptions.DiscreteGroupItems**. Denna metod kommer att tas bort 6 månader senare, från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| customGroupItems | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) | De anpassade gruppobjekten. |
| newField | boolean | Indikerar om ett nytt fält ska läggas till i pivottabellen |

**Returns:**
boolean -
### groupBy(double interval, boolean newField) {#groupBy-double-boolean-}
```
public void groupBy(double interval, boolean newField)
```


Gruppera fältet automatiskt med intervall.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden PivotField.Group(PivotFieldGroupOptions). Denna metod kommer att tas bort 6 månader senare, från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intervall | double | Den interna av gruppen. Automatiskt värde tilldelas om det är noll, |
| newField | boolean | Indikerar om ett nytt fält ska läggas till i pivottabellen. Endast för DateTime-grupp. |

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public boolean groupBy(double start, double end, double interval, boolean newField)
```


Gruppera filen efter nummer.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden PivotField.Group(PivotFieldGroupOptions). Denna metod kommer att tas bort 6 månader senare, från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | double | Startvärdet |
| end | double | Slutvärdet |
| intervall | double | Intervallet |
| newField | boolean | Indikerar om ett nytt fält ska läggas till i pivottabellen |

**Returns:**
boolean - False betyder att detta fält inte kan grupperas efter datum och tid.
### groupBy(int[] groups, double interval, boolean newField) {#groupBy-int---double-boolean-}
```
public void groupBy(int[] groups, double interval, boolean newField)
```


Gruppera fältet automatiskt internt.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden PivotField.Group(PivotFieldGroupOptions). Denna metod kommer att tas bort 6 månader senare, från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Grupptyper |
| intervall | double | Den interna av gruppen. Automatiskt värde tilldelas om det är noll, fungerar endast för gruppering efter tal eller dagar. |
| newField | boolean | Indikerar om ett nytt fält ska läggas till i pivottabellen. |

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


Döljer alla detaljer för varje pivåtelement.

### hideDetail(boolean isHiddenDetail) {#hideDetail-boolean-}
```
public void hideDetail(boolean isHiddenDetail)
```


Ställer in om detaljerna för alla PivotItems i ett pivottfält ska döljas. Det vill säga fäll ihop/expandera detta fält.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotItemsCollection.HideAllDetails() och UnhideAllDetails() metod. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isHiddenDetail | boolean | Om detaljerna för pivåtfältet ska döljas. |

### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


Ställer in om det specifika PivotItem i ett datafält är dolt.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotField.PivotItems[int].IsHidden egenskap. Denna metod kommer att tas bort 12 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | indexet för pivotItem i pivotField. |
| isHidden | boolean | om den specifika PivotItem är dold |

### hideItem(String itemValue, boolean isHidden) {#hideItem-java.lang.String-boolean-}
```
public void hideItem(String itemValue, boolean isHidden)
```


Ställer in om det specifika PivotItem i ett datafält är dolt.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotField.PivotItems[string].IsHidden egenskap. Denna metod kommer att tas bort 12 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| itemValue | java.lang.String | Namnet på pivotItem i pivotField. |
| isHidden | boolean | Om den specifika PivotItem är dold |

### hideItemDetail(int index, boolean isHiddenDetail) {#hideItemDetail-int-boolean-}
```
public void hideItemDetail(int index, boolean isHiddenDetail)
```


Ställer in om den specifika PivotItem i ett pivåtfält har dold detalj.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotField.PivotItems[int].IsDetailHidden egenskap. Denna metod kommer att tas bort 12 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | indexet för pivotItem i pivotField. |
| isHiddenDetail | boolean | om den specifika PivotItem är dold |

### initPivotItems() {#initPivotItems--}
```
public void initPivotItems()
```


Initiera pivåtelementen för pivåtfältet.

**Remarks**

OBS: Denna metod är nu föråldrad. Ta helt enkelt bort anropet av denna metod. Denna metod kommer att tas bort 6 månader senare från och med oktober 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### isAscendShow() {#isAscendShow--}
```
public boolean isAscendShow()
```


Indikerar om det angivna PivotTable-fältet automatiskt visas i stigande ordning.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.Top10AutoShowSettings.IsTop egenskap eller PivotField.Top10AutoShow() metod. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


Anger om objekten i detta pivåtfält är automatiskt sorterade stigande.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.SortSetting.SortType egenskap eller PivotField.SortBy() metod. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Anger om det angivna PivotTable-fältet visas automatiskt.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.Top10AutoShowSettings.IsAutoShow egenskap eller PivotField.Top10AutoShow() metod. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


Anger om objekten i detta PivotTable-fält är automatiskt sorterade.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.SortSetting.SortType egenskap eller PivotField.SortBy() metod. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isAutoSubtotals() {#isAutoSubtotals--}
```
public boolean isAutoSubtotals()
```


Anger om det angivna fältet visar automatiska delsummeringar. Standard är true.

**Returns:**
boolean
### isCalculatedField() {#isCalculatedField--}
```
public boolean isCalculatedField()
```


Anger om detta pivåtfält är ett beräknat fält.

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


Anger om det specifika PivotItem är dolt.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotField.PivotItems[int].IsHidden egenskap. Denna metod kommer att tas bort 12 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet för pivotItem i pivotField. |

**Returns:**
boolesk – om den specifika PivotItem är dold
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


Anger om detaljen för det specifika PivotItem ska döljas..

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotField.PivotItems[int].IsDetailHidden egenskap. Denna metod kommer att tas bort 12 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet för pivotItem i pivotField. |

**Returns:**
boolesk – om den specifika PivotItem är dold detalj
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


Anger om nya objekt ska inkluderas i fältet i manuellt filter. Standardvärdet är false.

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


Anger om sidbrytningar ska infogas efter varje objekt. Standardvärdet är false.

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


Anger om flera objekt kan väljas i sidfältet. Standardvärdet är false.

**Remarks**

Endast för sid (filter) fält.

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


Anger om etiketter för fältet ska upprepas i rad- eller kolumnregionen. Standardvärdet är false.

**Returns:**
boolean
### isValueFields() {#isValueFields--}
```
public boolean isValueFields()
```


Anger om detta fält representerar värdefält.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotField.IsValuesField egenskap. Denna metod kommer att tas bort 12 månader senare från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isValuesField() {#isValuesField--}
```
public boolean isValuesField()
```


Anger om detta fält representerar värdefält.

**Remarks**

Fungerar endast när det finns två eller fler datafält i pivottabellvyn.

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


Anger om det angivna fältet kan dras till kolumnområdet. Standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowDraggingToData(boolean value) {#setAllowDraggingToData-boolean-}
```
public void setAllowDraggingToData(boolean value)
```


Anger om det angivna fältet kan dras till värdeområdet. Standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowDraggingToPage(boolean value) {#setAllowDraggingToPage-boolean-}
```
public void setAllowDraggingToPage(boolean value)
```


Anger om det angivna fältet kan dras till sidområdet. Standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowDraggingToRow(boolean value) {#setAllowDraggingToRow-boolean-}
```
public void setAllowDraggingToRow(boolean value)
```


Anger om det angivna fältet kan dras till radregionen. Standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowRemovingFromView(boolean value) {#setAllowRemovingFromView-boolean-}
```
public void setAllowRemovingFromView(boolean value)
```


Anger om detta pivottfält kan tas bort från PivotTable-vyn. Standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAscendShow(boolean value) {#setAscendShow-boolean-}
```
public void setAscendShow(boolean value)
```


Indikerar om det angivna PivotTable-fältet automatiskt visas i stigande ordning.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.Top10AutoShowSettings.IsTop egenskap eller PivotField.Top10AutoShow() metod. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


Anger om objekten i detta pivåtfält är automatiskt sorterade stigande.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.SortSetting.SortType egenskap eller PivotField.SortBy() metod. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Anger om det angivna PivotTable-fältet visas automatiskt.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.Top10AutoShowSettings.IsAutoShow egenskap eller PivotField.Top10AutoShow() metod. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Representerar antalet översta eller nedersta objekt som automatiskt visas i det angivna PivotTable-fältet.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.Top10AutoShowSettings.AutoShowCount eller metoden PivotField.Top10AutoShow() istället. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


Representerar index för automatisk visning av fält. -1 betyder PivotField själv. Det bör vara indexet för datafälten.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.Top10AutoShowSettings.RankBy eller metoden PivotField.Top10AutoShow() istället. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


Anger om objekten i detta PivotTable-fält är automatiskt sorterade.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.SortSetting.SortType egenskap eller PivotField.SortBy() metod. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


Representerar indexet för fältet som sorteras automatiskt. -1 betyder PivotField själv, andra betyder positionen för datafälten.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.SortSetting.SortBy eller metoden PivotField.SortBy() istället. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


Anger om det angivna fältet visar automatiska delsummeringar. Standard är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


Representerar indexet i källpivotfälten.

**Remarks**

OBS: Denna setter för egenskapen är nu föråldrad. Denna setter för egenskapen kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


Ställer in det för närvarande visade sidobjektet för detta pivåtfält (endast sidfält).

**Remarks**

Använd [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) som sentinelvärde för att indikera \"Select All\". Detta är en fördefinierad markör och är inte ett giltigt objektindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | short |  |

### setCurrentPageItemText(String value) {#setCurrentPageItemText-java.lang.String-}
```
public void setCurrentPageItemText(String value)
```


Hämtar visningstexten för det aktuella sidobjektet för detta pivottfält (endast sidfält).

**Remarks**

Returnerar \"(All)\" när [getCurrentPageItem()](../../com.aspose.cells/pivotfield\\#getCurrentPageItem--) är lika med [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX). För andra värden returneras strängrepresentationen av objektindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Representerar visningsnamnet för pivottfältet i pivottabellvyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


Anger om det angivna fältet kan dras till kolumnområdet. Standardvärdet är sant.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.AllowDraggingToColumn. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


Anger om det angivna fältet kan dras till värdeområdet. Standardvärdet är sant.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.AllowDraggingToData. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


Anger om detta pivottfält kan tas bort från PivotTable-vyn. Standardvärdet är sant.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.AllowRemovingFromView. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


Anger om det angivna fältet kan dras till sidområdet. Standardvärdet är sant.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.AllowDraggingToPage. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


Anger om det angivna fältet kan dras till radregionen. Standardvärdet är sant.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.AllowDraggingToRow. Denna metod kommer att tas bort 12 månader senare, från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


Representerar funktionen som används för att sammanfatta detta PivotTable-datafält.

Se [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


Anger om nya objekt ska inkluderas i fältet i manuellt filter. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


Anger om en tom rad ska infogas efter varje objekt. Endast för radfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


Anger om sidbrytningar ska infogas efter varje objekt. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


Anger om flera objekt kan väljas i sidfältet. Standardvärdet är false.

**Remarks**

Endast för sid (filter) fält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Representerar namnet på PivotField.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


Anger om en sorteringsoperation som kommer att tillämpas på detta pivottfält är en autosortering eller en enkel datasortering.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen !PivotField.SortSetting.IsSimpleSort. Denna metod kommer att tas bort 12 månader senare, från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Representerar det inbyggda visningsformatet för tal och datum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Representerar det anpassade visningsformatet för tal och datum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


Anger om etiketter för fältet ska upprepas i rad- eller kolumnregionen. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Anger om alla objekt ska visas i PivotTable-vyn, även om de inte innehåller sammanfattningsdata. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


Anger om etiketter för nästa fält ska visas i samma kolumn i Pivot Table-vyn. Endast för radfält.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället egenskapen PivotField.ShowInCompactForm. Denna metod kommer att tas bort 12 månader senare, från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowInCompactForm(boolean value) {#setShowInCompactForm-boolean-}
```
public void setShowInCompactForm(boolean value)
```


Ställer in ett värde som indikerar om detta radfält använder kompakt formulärlayout. Gäller endast radfält.

**Remarks**

Kompakt form är ett delläge av kontur-layout. Denna inställning har bara effekt när [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


Ställer in ett värde som indikerar om detta radfält använder konturlayout. Gäller endast radfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


Anger om delsummer ska visas högst upp eller längst ner på objekten.

**Remarks**

Fungerar endast för pivåtfält i radregionen när ShowInOutlineForm är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSubtotals(int value) {#setSubtotals-int-}
```
public void setSubtotals(int value)
```


Ställer in delsummerna för fältet. Endast för rad- eller kolumnpivotfält.

Se [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Ställer in hur det angivna fältet ska delsummeras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| visad | boolean | Om det angivna fältet visar dessa delsummer. |

### showAllDetails() {#showAllDetails--}
```
public void showAllDetails()
```


Visa alla detaljer för varje pivåtelement.

### showValuesAs(int showValuesAsType, int baseField, int baseItem) {#showValuesAs-int-int-int-}
```
public void showValuesAs(int showValuesAsType, int baseField, int baseItem)
```


Ställer in beräkningen "Show Values As" för detta pivåtfält.

**Remarks**

Endast för datafält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Typ av "Show Values As"-beräkning. |
| baseField | int | Index för basfältet som används för beräkningen. |
| baseItem | int | Index för basobjektet för beräkningen. Använd [PivotShowValuesSetting.PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) för föregående objekt, [PivotShowValuesSetting.NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) för efterföljande objekt; icke\\u9225\\u6182egativa värden betecknar det ordningsmässiga indexet för ett specifikt pivotobjekt. |

### showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem) {#showValuesAs-int-int-int-int-}
```
public void showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)
```


Visar värden för datafältet i annat displayformat när beräkningen ShowDataAs används.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.ShowValuesAs(PivotShowValuesAsType,int,int)-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| displayFormat | int | [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat). Datavisningsformatstypen. |
| baseField | int | Indexet till fältet som ShowDataAs-beräkningen baseras på. |
| baseItemPositionType | int | [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype). Positionstypen för basobjektet. |
| baseItem | int | Indexet till basobjektet som ShowDataAs-beräkningen baseras på. Fungerar endast när baseItemPositionType är anpassad. |

### showValuesAs(int showValuesAsType, String baseField, String baseItem) {#showValuesAs-int-java.lang.String-java.lang.String-}
```
public void showValuesAs(int showValuesAsType, String baseField, String baseItem)
```


Konfigurerar beräkningen "Show Values As" för detta datafält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Beräkningstypen för Show Values As. |
| baseField | java.lang.String | Namnet på basfältet som används i beräkningen. |
| baseItem | java.lang.String | Rubrik för ett vanligt pivotobjekt. Accepterar också reserverade nyckelord: `(previous)` för föregående objekt, `(next)` för nästa objekt. Skicka `null` om den valda beräkningstypen inte kräver ett basobjekt. |

### sortBy(int sortType) {#sortBy-int-}
```
public void sortBy(int sortType)
```


Sorterar detta pivåtfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Sorteringstypen för detta fält. |

### sortBy(int sortType, int fieldSortedBy) {#sortBy-int-int-}
```
public void sortBy(int sortType, int fieldSortedBy)
```


Sorterar detta pivåtfält.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.SortBy(SortOrder, int,string)-metoden eller PivotField.IsAutoSort-egenskapen. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Sorteringstypen för detta fält. |
| fieldSortedBy | int | Indexet för pivotfältet som sorteras efter. -1 betyder sortering efter datalabels för detta fält, andra värden betyder indexet för datafältet som sorteras efter. |

### sortBy(int sortType, int fieldSortedBy, int dataType, String cellName) {#sortBy-int-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)
```


Sorterar detta pivåtfält.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.SortBy(SortOrder, int,string)-metoden. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Sorteringstypen för detta fält. |
| fieldSortedBy | int | Indexet för pivotfältet som sorteras efter. -1 betyder sortering efter datalabels för detta fält, andra värden betyder indexet för datafältet som sorteras efter. |
| dataType | int | [PivotLineType](../../com.aspose.cells/pivotlinetype). Typen av data som sorteras efter. |
| cellNamn | java.lang.String | Sortera efter värden i raden eller kolumnen |

### sortBy(int sortType, int fieldSortedBy, String cellName) {#sortBy-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, String cellName)
```


Sorterar detta pivåtfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Sorteringstypen för detta fält. |
| fieldSortedBy | int | Indexet för pivotfältet som sorteras efter. -1 betyder sortering efter datalabels för detta fält, andra värden betyder indexet för datafältet som sorteras efter. |
| cellNamn | java.lang.String | Sortera efter värden i raden eller kolumnen. Om Null, gruppera efter fältets total, annars gruppera efter värden i den valda kolumnen eller raden. |

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


Konfigurerar Top10 AutoShow-inställningarna för detta pivåtfält.

**Remarks**

Den här metoden konfigurerar . XLS binärformat: AutoShow (Top10) är det inbyggda och enda stödda alternativet. XLSX (OpenXML): Det underliggande filformatet stöder Top10 AutoShow, men Excel 2007 och senare användargränssnitt visar detta endast via Top10-filter. Om XLS‑kompatibilitet inte krävs rekommenderas att använda Top10-filter istället.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAutoShow | boolean | true för att aktivera AutoShow; false för att inaktivera. |
| isTop | boolean | Om true visas de översta objekten; false visas de nedersta objekten. |
| antal | int | Antal översta/nedersta objekt att visa. |
| rankBy | int | Index för datafält som används för rangordning. Använd -1 för att rangordna efter pivotelementets egna värden. |

### ungroup() {#ungroup--}
```
public void ungroup()
```


Avgruppera pivåtfältet.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

