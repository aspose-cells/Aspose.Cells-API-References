---
title: "GridWorksheet"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar ett enskilt kalkylblad."
type: docs
url: /sv/java/com.aspose.gridweb/gridworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class GridWorksheet extends Control
```

Inkapslar objektet som representerar ett enskilt kalkylblad.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addAutoFilter(int row, int startColumn, int endColumn)](#addAutoFilter-int-int-int-) | Ställer in intervallet som det angivna AutoFiltret gäller för. |
| [addCustomFilter(int row, String critira)](#addCustomFilter-int-java.lang.String-) | Lägg till anpassat filter för den angivna raden. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Anpassar automatiskt kolumnbredden. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Anpassar automatiskt kolumnbredden. |
| [autoFitColumns()](#autoFitColumns--) |  |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Anpassar automatiskt radhöjden. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Anpassar automatiskt radhöjden. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Anpassar automatiskt radhöjden i ett rektangulärt område. |
| [autoFitRows()](#autoFitRows--) | Anpassar automatiskt alla rader i detta kalkylblad. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Anpassar automatiskt alla rader i detta kalkylblad. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Anpassar automatiskt radhöjden i ett område. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Beräknar en formel. |
| [clearComments()](#clearComments--) | Rensar alla kommentarer i designerns kalkylblad. |
| [copy(GridWorksheet sourceSheet)](#copy-com.aspose.gridweb.GridWorksheet-) | Kopierar innehåll och format från ett annat kalkylblad. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)](#createSubtotal-int-int-int-int-int---) | Skapar delsumma i bladet. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Skapar delsumma i bladet. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterString(int column, String criteria)](#filterString-int-java.lang.String-) | Ställer in filtret för kolumnen. Observera att vi ska anropa AddAutoFilter innan vi anropar filterString. Filterkriteriesträngen. Observera att vi använder kommatecken -> "," som avgränsare, så cellvärdet du vill filtrera får inte innehålla kommatecken. filterString(10,"123,456") betyder att kolumn 10 ska innehålla 123 eller 456, filterString(10,"123") betyder att kolumn 10 ska innehålla 123. Kolumnindexvärdet separeras med kommatecken, t.ex. 123,456,789 eller abc |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [getActiveCell()](#getActiveCell--) | Hämtar den aktiva cellen i kalkylbladet. |
| [getBackgroundImage()](#getBackgroundImage--) | Hämtar kalkylbladets bakgrundsbild. |
| [getCells()](#getCells--) | Hämtar [GridCell](../../com.aspose.gridweb/gridcell)-samlingen. |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Representerar kalkylbladets kodnamn. |
| [getColumnCaption(int column)](#getColumnCaption-int-) | Hämtar kolumnrubriken. |
| [getColumnHeaderToolTip(int colIndex)](#getColumnHeaderToolTip-int-) | Hämtar verktygstipstexten för kolumnrubriken. |
| [getColumnReadonly(int columnIndex)](#getColumnReadonly-int-) | Hämtar om en kolumn är skrivskyddad. |
| [getComments()](#getComments--) | Hämtar [GridComment](../../com.aspose.gridweb/gridcomment)-samlingen. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Anger om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. |
| [getDisplayZeros()](#getDisplayZeros--) | Sant om nollvärden visas. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Representerar första synliga kolumnindex. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Representerar första synliga radindex. |
| [getFreezedPanes()](#getFreezedPanes--) | Hämtar frysade rutor. |
| [getGridActiveCell()](#getGridActiveCell--) | Hämtar den aktiva cellen i kalkylbladet. |
| [getHyperlinks()](#getHyperlinks--) | Hämtar [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)-samlingen. |
| [getIndex()](#getIndex--) | Hämtar indexet för bladet i kalkylblads‑samlingen. |
| [getIsReadonly(int row, int col)](#getIsReadonly-int-int-) | Hämtar om cellen är skrivskyddad. Detta är ett utökat attribut för GridWeb, det sparas inte i den faktiska Excel-filen. |
| [getName()](#getName--) | Hämtar namnet på kalkylbladet. |
| [getOutlineShown()](#getOutlineShown--) | Anger om kontur ska visas. |
| [getPictures()](#getPictures--) | Hämtar en [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) samling. |
| [getPivotTables()](#getPivotTables--) | Hämtar pivottabellerna i kalkylbladet. |
| [getRowCaption(int row)](#getRowCaption-int-) | Hämtar radrubriken. |
| [getRowHeaderToolTip(int rowIndex)](#getRowHeaderToolTip-int-) | Hämtar radhuvudets verktygstipstext. |
| [getRowReadonly(int rowIndex)](#getRowReadonly-int-) | Hämtar om en rad är skrivskyddad. |
| [getSelected()](#getSelected--) | Anger om detta kalkylblad är valt när arbetsboken öppnas. |
| [getShapes()](#getShapes--) | Hämtar en [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) samling. |
| [getStandardHeight()](#getStandardHeight--) | Hämtar standardradens höjd i detta kalkylblad,i enheten punkter. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Hämtar standardradens höjd i detta kalkylblad,i enheten pixlar. |
| [getTabColor()](#getTabColor--) | Representerar flikfärgen för kalkylbladet. |
| [getUniqueID()](#getUniqueID--) | Hämtar UniqueID i kontrollen |
| [getValidations()](#getValidations--) | Hämtar samlingen av datavalideringsinställningar i kalkylbladet. |
| [getVisible()](#getVisible--) | Anger om detta bladnamn visas i bladflikarna i kontrollen. |
| [getWorkbook()](#getWorkbook--) | Hämtar [GridWorkbook](../../com.aspose.gridweb/gridworkbook) objektet för kalkylbladssamlingen. |
| [getZoom()](#getZoom--) | Representerar skalningsfaktorn i procent. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Grupperar rader. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Hämtar ett värde som anger om rutnätslinjerna är synliga. Standard är true. |
| [isProtected()](#isProtected--) | Anger om kalkylbladet är skyddat. |
| [isSummaryRowBelow()](#isSummaryRowBelow--) | Anger om sammanfattningsraden kommer att placeras under detaljraderna i dispositionen. |
| [moveTo(int index)](#moveTo-int-) | Flyttar bladet till en annan plats i kalkylarket. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshFilter()](#refreshFilter--) | Uppdatera autofilter för att dölja eller visa raderna. |
| [removeAutoFilter()](#removeAutoFilter--) | Ta bort autofiltret i kalkylbladet. |
| [removeSubtotal()](#removeSubtotal--) | Tar bort delsumma som skapats av metoden CreateSubtotal i bladet. |
| [resetFilter(int fieldIndex)](#resetFilter-int-) | Det heltalsavståndet för fältet som du vill tillämpa ,baserat på den första filterkolumnen (från vänster i listan; det vänstra fältet är fält 0). |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Ställer in den aktiva cellen i kalkylbladet. |
| [setAllCellsEditable()](#setAllCellsEditable--) | Gör alla celler redigerbara.det är ett utökat attribut |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Gör alla celler skrivskyddade.det är ett utökat attribut observera att detta attribut inte kan behållas i faktiska celler, om du vill behålla skyddet använd setProtect |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Ställer in bakgrundsbild för kalkylbladet. |
| [setColumnCaption(int column, String caption)](#setColumnCaption-int-java.lang.String-) | Ställer in rubriken för kolumnen. observera att detta är ett utökat attribut och kan inte behållas i excelfil |
| [setColumnHeaderToolTip(int colIndex, String toolTip)](#setColumnHeaderToolTip-int-java.lang.String-) | Ställer in kolumnhuvudets verktygstipstext. |
| [setColumnReadonly(int columnIndex, boolean isReadonly)](#setColumnReadonly-int-boolean-) | Ställer in en kolumn som skrivskyddad så att användaren inte kan ta bort den från klientsidan. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Anger om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Sant om nollvärden visas. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Gör ett område av celler redigerbara. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör alla celler skrivskyddade genom att anropa SetAllCellsReadonly method. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Representerar första synliga kolumnindex. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Representerar första synliga radindex. |
| [setGridActiveCell(GridCell value)](#setGridActiveCell-com.aspose.gridweb.GridCell-) | Ställer in den aktiva cellen i kalkylbladet. |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Ställer in ett värde som anger om rutnätslinjerna är synliga. Standard är true. |
| [setIsReadonly(int row, int col, boolean value)](#setIsReadonly-int-int-boolean-) | Ställer in om cellen är skrivskyddad.det är ett utökat attribut för GridWeb ,det kommer inte att behållas i den faktiska excel file |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på kalkylbladet. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Anger om kontur ska visas. |
| [setProtect()](#setProtect--) | Skyddar kalkylbladet. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Gör ett område av celler skrivskyddade. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells First make all cells editable by calling the SetAllCellsEditable method. |
| [setRowCaption(int row, String caption)](#setRowCaption-int-java.lang.String-) | Ställer in rubriken för raden. |
| [setRowHeaderToolTip(int rowIndex, String toolTip)](#setRowHeaderToolTip-int-java.lang.String-) | Ställer in radhuvudets verktygstipstext. |
| [setRowReadonly(int rowIndex, boolean isReadonly)](#setRowReadonly-int-boolean-) | Ställer in en rad som skrivskyddad så att användaren inte kan ta bort den från klientsidan. |
| [setSelected(boolean value)](#setSelected-boolean-) | Anger om detta kalkylblad är valt när arbetsboken öppnas. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Ställer in standardradens höjd i detta kalkylblad,i enheten punkter. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Ställer in standardradens höjd i detta kalkylblad,i enheten pixlar. |
| [setSummaryRowBelow(boolean value)](#setSummaryRowBelow-boolean-) | Anger om sammanfattningsraden kommer att placeras under detaljraderna i dispositionen. |
| [setTabColor(Color value)](#setTabColor-com.aspose.gridweb.Color-) | Representerar flikfärgen för kalkylbladet. |
| [setVisible(boolean value)](#setVisible-boolean-) | Anger om detta bladnamn visas i bladflikarna i kontrollen. |
| [setZoom(int value)](#setZoom-int-) | Representerar skalningsfaktorn i procent. |
| [toString()](#toString--) |  |
| [unFreezePanes()](#unFreezePanes--) | Låser upp paneler i kalkylbladet. |
| [unGroupRows(int firstIndex, int lastIndex)](#unGroupRows-int-int-) | Avgrupperar rader. |
| [unProtect()](#unProtect--) | unProtects kalkylbladet. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAutoFilter(int row, int startColumn, int endColumn) {#addAutoFilter-int-int-int-}
```
public void addAutoFilter(int row, int startColumn, int endColumn)
```


Ställer in intervallet som det angivna AutoFiltret gäller för.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| startColumn | int | Startkolumnens index. |
| endColumn | int | Slutkolumnindex. |

### addCustomFilter(int row, String critira) {#addCustomFilter-int-java.lang.String-}
```
public void addCustomFilter(int row, String critira)
```


Lägg till anpassat filter för den angivna raden.

**Remarks**

Filterkriteriesträngen. Observera att vi använder , och ; som avgränsningstecken, så cellvärdet får inte innehålla dessa avgränsningstecken. Nedan är exempel på kriteriesträngar //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int |  |
| critira | java.lang.String |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Anpassar automatiskt kolumnbredden.

**Remarks**

AutoFitColumn är en inexakt funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Anpassar automatiskt kolumnbredden.

**Remarks**

Denna metod anpassar automatiskt en rad baserat på innehållet i ett cellintervall inom raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| firstRow | int | Första radens index. |
| lastRow | int | Sista radens index. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```




### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Anpassar automatiskt radhöjden.

**Remarks**

AutoFitRow är en inexakt funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Anpassar automatiskt radhöjden.

**Remarks**

Denna metod anpassar automatiskt en rad baserat på innehållet i ett cellintervall inom raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |
| firstColumn | int | Första kolumnens index. |
| lastColumn | int | Sista kolumnens index. |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Anpassar automatiskt radhöjden i ett rektangulärt område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| slutRad | int | Slutradens index. |
| startColumn | int | Startkolumnens index. |
| endColumn | int | Slutkolumnens index. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Anpassar automatiskt alla rader i detta kalkylblad.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Anpassar automatiskt alla rader i detta kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| onlyAuto | boolean | True, endast autofitar radens höjd när radens höjd inte är anpassad. |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Anpassar automatiskt radhöjden i ett område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| slutRad | int | Slutradens index. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Beräknar en formel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String |  |

**Returns:**
java.lang.Object - 
### clearComments() {#clearComments--}
```
public void clearComments()
```


Rensar alla kommentarer i designerns kalkylblad.

### copy(GridWorksheet sourceSheet) {#copy-com.aspose.gridweb.GridWorksheet-}
```
public void copy(GridWorksheet sourceSheet)
```


Kopierar innehåll och format från ett annat kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Källkalkylblad. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList) {#createSubtotal-int-int-int-int-int---}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)
```


Skapar delsumma i bladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnNameRowIndex | int | Radindex för kolumnnamnsraden. |
| dataRows | int | Antalet datarader. |
| groupByColumnIndex | int | Kolumnindex för den kolumn som ska grupperas. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Subtotal-funktionstypen. |
| subtotalColumnIndexList | int[] | Kolumnindex som ska summeras. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Skapar delsumma i bladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnNameRowIndex | int | Radindex för kolumnnamnsraden. |
| dataRows | int | Antalet datarader. |
| groupByColumnIndex | int | Kolumnindex för den kolumn som ska grupperas. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Subtotal-funktionstypen. |
| subtotalColumnIndexList | int[] | Kolumnindex som ska summeras. |
| functionLabel | java.lang.String | Etiketten för subtotalfunktionen. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Stilen för totalraden. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Stilen för subtotalraden. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). Nummertypen för subtotalresultatcellerna. |
| customString | java.lang.String | Den anpassade formatsträngen för subtotalresultatcellerna. Kan vara null. |

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
### filterString(int column, String criteria) {#filterString-int-java.lang.String-}
```
public void filterString(int column, String criteria)
```


Ställer in filtret för kolumnen. Observera att vi ska anropa AddAutoFilter innan vi anropar filterString. Filterkriteriesträngen. Observera att vi använder kommatecken -> "," som avgränsare, så cellvärdet du vill filtrera får inte innehålla kommatecken. filterString(10,"123,456") betyder att kolumn 10 ska innehålla 123 eller 456, filterString(10,"123") betyder att kolumn 10 ska innehålla 123. Kolumnindexvärdet separeras med kommatecken, t.ex. 123,456,789 eller abc

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int |  |
| kriterier | java.lang.String |  |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Fryser rutor vid den angivna cellen i kalkylbladet.

**Remarks**

Radindex och kolumnindex kan inte alla vara noll. Antalet rader och antalet kolumner kan inte heller alla vara noll.

De två första parametrarna anger den frysta positionen och de två sista parametrarna anger området som är fryst i det övre vänstra fönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| kolumn | int | Kolumnindex. |
| freezedRows | int | Antal synliga rader i övre fönstret, högst lika med radindex. |
| freezedColumns | int | Antalet synliga kolumner i vänsterpanelen, högst kolumnindexet. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Fryser rutor vid den angivna cellen i kalkylbladet.

**Remarks**

Radindex och kolumnindex kan inte alla vara noll. Antalet rader och antalet kolumner kan inte heller alla vara noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn. |
| freezedRows | int | Antal synliga rader i övre fönstret, högst lika med radindex. |
| freezedColumns | int | Antalet synliga kolumner i vänsterpanelen, högst kolumnindexet. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Hämtar den aktiva cellen i kalkylbladet.

**Returns:**
java.lang.String
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Hämtar kalkylbladets bakgrundsbild.

**Returns:**
byte[]
### getCells() {#getCells--}
```
public GridCells getCells()
```


Hämtar [GridCell](../../com.aspose.gridweb/gridcell)-samlingen.

**Returns:**
[GridCells](../../com.aspose.gridweb/gridcells)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Representerar kalkylbladets kodnamn.

**Remarks**

Du kan inte ändra kodnamnet medan mallfilen innehåller VBA/makro.

**Returns:**
java.lang.String
### getColumnCaption(int column) {#getColumnCaption-int-}
```
public String getColumnCaption(int column)
```


Hämtar kolumnrubriken. Om rubriken inte är angiven returneras en tom sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |

**Returns:**
java.lang.String - Kolumnrubriken. Om rubriken inte är angiven returneras en tom sträng.
### getColumnHeaderToolTip(int colIndex) {#getColumnHeaderToolTip-int-}
```
public String getColumnHeaderToolTip(int colIndex)
```


Hämtar verktygstipstexten för kolumnrubriken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| colIndex | int | Kolumnens index. |

**Returns:**
java.lang.String - Verktygstipstexten.
### getColumnReadonly(int columnIndex) {#getColumnReadonly-int-}
```
public boolean getColumnReadonly(int columnIndex)
```


Hämtar om en kolumn är readonly. detta är en utökad metod för GridWeb specifikt, den kommer inte att behållas och påverka den faktiska Excel-filen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | kolumnindex. |

**Returns:**
boolean - Om readonly returnerar true.
### getComments() {#getComments--}
```
public GridCommentCollection getComments()
```


Hämtar [GridComment](../../com.aspose.gridweb/gridcomment)-samlingen.

**Returns:**
[GridCommentCollection](../../com.aspose.gridweb/gridcommentcollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Indikerar om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. Standard är falskt.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


Sant om nollvärden visas.

**Returns:**
boolean
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


Representerar första synliga kolumnindex.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


Representerar första synliga radindex.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Hämtar frysade rutor.

**Returns:**
int[] - Returnerar null betyder att kalkylbladet inte är fryst 0:Radindex;1:kolumn;2:frysta rader;3:frysta rader
### getGridActiveCell() {#getGridActiveCell--}
```
public GridCell getGridActiveCell()
```


Hämtar den aktiva cellen i kalkylbladet.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHyperlinks() {#getHyperlinks--}
```
public GridHyperlinkCollection getHyperlinks()
```


Hämtar [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)-samlingen.

**Returns:**
[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Hämtar indexet för bladet i kalkylblads‑samlingen.

**Returns:**
int
### getIsReadonly(int row, int col) {#getIsReadonly-int-int-}
```
public boolean getIsReadonly(int row, int col)
```


Hämtar om cellen är skrivskyddad. Detta är ett utökat attribut för GridWeb, det sparas inte i den faktiska Excel-filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int |  |
| kol | int |  |

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på kalkylbladet.

**Remarks**

Den maximala längden för bladnamn är 31. Du kan inte tilldela samma namn (skiftlägesokänsligt) till två kalkylblad. Till exempel kan du inte sätta "SheetName1" på det första kalkylbladet och sätta "SHEETNAME1" på det andra kalkylbladet.

**Returns:**
java.lang.String
### getOutlineShown() {#getOutlineShown--}
```
public boolean getOutlineShown()
```


Anger om kontur ska visas.

**Returns:**
boolean
### getPictures() {#getPictures--}
```
public GridPictureCollection getPictures()
```


Hämtar en [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) samling.

**Returns:**
[GridPictureCollection](../../com.aspose.gridweb/gridpicturecollection)
### getPivotTables() {#getPivotTables--}
```
public GridPivotTableCollection getPivotTables()
```


Hämtar pivottabellerna i kalkylbladet.

**Returns:**
[GridPivotTableCollection](../../com.aspose.gridweb/gridpivottablecollection)
### getRowCaption(int row) {#getRowCaption-int-}
```
public String getRowCaption(int row)
```


Hämtar radens rubrik. Om rubriken inte är angiven returneras en tom sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |

**Returns:**
java.lang.String - Radens rubrik. Om rubriken inte är angiven returneras en tom sträng.
### getRowHeaderToolTip(int rowIndex) {#getRowHeaderToolTip-int-}
```
public String getRowHeaderToolTip(int rowIndex)
```


Hämtar radhuvudets verktygstipstext.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radens index. |

**Returns:**
java.lang.String - Verktygstipstexten.
### getRowReadonly(int rowIndex) {#getRowReadonly-int-}
```
public boolean getRowReadonly(int rowIndex)
```


Hämtar om en rad är readonly. detta är en utökad metod för GridWeb specifikt, den kommer inte att behållas och påverka den faktiska Excel-filen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | radindex. |

**Returns:**
boolean - Om readonly returnerar true.
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


Anger om detta kalkylblad är valt när arbetsboken öppnas.

**Returns:**
boolean
### getShapes() {#getShapes--}
```
public GridShapeCollection getShapes()
```


Hämtar en [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) samling.

**Returns:**
[GridShapeCollection](../../com.aspose.gridweb/gridshapecollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Hämtar standardradens höjd i detta kalkylblad,i enheten punkter.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Hämtar standardradens höjd i detta kalkylblad,i enheten pixlar.

**Returns:**
int
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Representerar flikfärgen för kalkylbladet.

**Remarks**

Denna funktion stöds endast i ExcelXP (Excel2002) och senare versioner. Om du sparar filen som Excel97- eller Excel2000-format kommer den att utelämnas.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Hämtar UniqueID i kontrollen

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Hämtar samlingen av datavalideringsinställningar i kalkylbladet.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Anger om detta bladnamn visas i bladflikarna i kontrollen.

**Returns:**
boolean
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


Hämtar [GridWorkbook](../../com.aspose.gridweb/gridworkbook) objektet för kalkylbladssamlingen.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400.

**Returns:**
int
### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Grupperar rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska grupperas. |
| lastIndex | int | Det sista radindexet som ska grupperas. |
| isHidden | boolean | Anger om de grupperade raderna är dolda. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Hämtar ett värde som anger om rutnätslinjerna är synliga. Standard är true.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Anger om kalkylbladet är skyddat.

**Returns:**
boolean
### isSummaryRowBelow() {#isSummaryRowBelow--}
```
public boolean isSummaryRowBelow()
```


Anger om sammanfattningsraden kommer att placeras under detaljraderna i dispositionen.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Flyttar bladet till en annan plats i kalkylarket.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Destinationsbladets index. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshFilter() {#refreshFilter--}
```
public void refreshFilter()
```


Uppdatera autofilter för att dölja eller visa raderna.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Ta bort autofiltret i kalkylbladet.

### removeSubtotal() {#removeSubtotal--}
```
public void removeSubtotal()
```


Tar bort delsumma som skapats av metoden CreateSubtotal i bladet.

### resetFilter(int fieldIndex) {#resetFilter-int-}
```
public void resetFilter(int fieldIndex)
```


Det heltalsavståndet för fältet som du vill tillämpa ,baserat på den första filterkolumnen (från vänster i listan; det vänstra fältet är fält 0).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int |  |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Ställer in den aktiva cellen i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Gör alla celler redigerbara.det är ett utökat attribut

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Gör alla celler skrivskyddade.det är ett utökat attribut observera att detta attribut inte kan behållas i faktiska celler, om du vill behålla skyddet använd setProtect

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Ställer in bakgrundsbild för kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte[] |  |

### setColumnCaption(int column, String caption) {#setColumnCaption-int-java.lang.String-}
```
public void setColumnCaption(int column, String caption)
```


Ställer in rubriken för kolumnen. observera att detta är ett utökat attribut och kan inte behållas i excelfil

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| rubrik | java.lang.String | Kolumnens rubrik. Skicka null eller en tom sträng om du vill avbryta rubriken. |

### setColumnHeaderToolTip(int colIndex, String toolTip) {#setColumnHeaderToolTip-int-java.lang.String-}
```
public void setColumnHeaderToolTip(int colIndex, String toolTip)
```


Ställer in kolumnhuvudets verktygstipstext.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| colIndex | int | Kolumnens index. |
| verktygstips | java.lang.String | Verktygstexten. |

### setColumnReadonly(int columnIndex, boolean isReadonly) {#setColumnReadonly-int-boolean-}
```
public void setColumnReadonly(int columnIndex, boolean isReadonly)
```


Ställer in en kolumn som readonly så att användaren inte kan ta bort den från klientsidan. detta är en utökad metod för GridWeb specifikt, den kommer inte att behållas och påverka den faktiska Excel-filen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | kolumnindex. |
| isReadonly | boolean | true eller false. |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Indikerar om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. Standard är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


Sant om nollvärden visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Gör ett cellområde redigerbart. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör alla celler skrivskyddade genom att anropa metoden SetAllCellsReadonly. Anropa sedan den här metoden för att ange vilka celler som ska vara redigerbara

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startraden för intervallet. |
| startColumn | int | Startkolumnen för intervallet. |
| rader | int | Antalet rader. |
| kolumner | int | Antalet kolumner. |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


Representerar första synliga kolumnindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


Representerar första synliga radindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setGridActiveCell(GridCell value) {#setGridActiveCell-com.aspose.gridweb.GridCell-}
```
public void setGridActiveCell(GridCell value)
```


Ställer in den aktiva cellen i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Ställer in ett värde som anger om rutnätslinjerna är synliga. Standard är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIsReadonly(int row, int col, boolean value) {#setIsReadonly-int-int-boolean-}
```
public void setIsReadonly(int row, int col, boolean value)
```


Ställer in om cellen är skrivskyddad.det är ett utökat attribut för GridWeb ,det kommer inte att behållas i den faktiska excel file

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int |  |
| kol | int |  |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på kalkylbladet.

**Remarks**

Den maximala längden för bladnamn är 31. Du kan inte tilldela samma namn (skiftlägesokänsligt) till två kalkylblad. Till exempel kan du inte sätta "SheetName1" på det första kalkylbladet och sätta "SHEETNAME1" på det andra kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Anger om kontur ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setProtect() {#setProtect--}
```
public void setProtect()
```


Skyddar kalkylbladet.

**Remarks**

Denna metod skyddar kalkylbladet utan lösenord. Den kan skydda kalkylbladet i alla versioner av Excel-filen.

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Gör ett cellområde readonly. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör först alla celler redigerbara genom att anropa metoden SetAllCellsEditable. Anropa sedan den här metoden för för att ange vilka celler som ska vara readonly

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startraden för intervallet. |
| startColumn | int | Startkolumnen för intervallet. |
| rader | int | Antalet rader. |
| kolumner | int | Antalet kolumner. |

### setRowCaption(int row, String caption) {#setRowCaption-int-java.lang.String-}
```
public void setRowCaption(int row, String caption)
```


Ställer in rubriken för raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| rubrik | java.lang.String | Radens rubrik. Skicka null eller en tom sträng om du vill avbryta rubriken. |

### setRowHeaderToolTip(int rowIndex, String toolTip) {#setRowHeaderToolTip-int-java.lang.String-}
```
public void setRowHeaderToolTip(int rowIndex, String toolTip)
```


Ställer in radhuvudets verktygstipstext.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radens index. |
| verktygstips | java.lang.String | Verktygstexten. |

### setRowReadonly(int rowIndex, boolean isReadonly) {#setRowReadonly-int-boolean-}
```
public void setRowReadonly(int rowIndex, boolean isReadonly)
```


Ställer in en rad som readonly så att användaren inte kan ta bort den från klientsidan. detta är en utökad metod för GridWeb specifikt, den kommer inte att behållas och påverka den faktiska Excel-filen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | radindex. |
| isReadonly | boolean | true eller false. |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Anger om detta kalkylblad är valt när arbetsboken öppnas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Ställer in standardradens höjd i detta kalkylblad,i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Ställer in standardradens höjd i detta kalkylblad,i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSummaryRowBelow(boolean value) {#setSummaryRowBelow-boolean-}
```
public void setSummaryRowBelow(boolean value)
```


Anger om sammanfattningsraden kommer att placeras under detaljraderna i dispositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.gridweb.Color-}
```
public void setTabColor(Color value)
```


Representerar flikfärgen för kalkylbladet.

**Remarks**

Denna funktion stöds endast i ExcelXP (Excel2002) och senare versioner. Om du sparar filen som Excel97- eller Excel2000-format kommer den att utelämnas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Anger om detta bladnamn visas i bladflikarna i kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Låser upp paneler i kalkylbladet.

### unGroupRows(int firstIndex, int lastIndex) {#unGroupRows-int-int-}
```
public void unGroupRows(int firstIndex, int lastIndex)
```


Avgrupperar rader.

**Remarks**

Tar bara bort yttre gruppinformation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska avgrupperas. |
| lastIndex | int | Det sista radindexet som ska avgrupperas. |

### unProtect() {#unProtect--}
```
public void unProtect()
```


unProtects kalkylbladet.

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

