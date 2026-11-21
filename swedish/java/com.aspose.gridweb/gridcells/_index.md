---
title: "GridCells"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.gridweb/gridcells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class GridCells implements Iterable
```

Inkapslar en samling av [GridCell](../../com.aspose.gridweb/gridcell) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Hämtar cellnamnet enligt dess rad- och kolumnindex. |
| [cellNameToIndex(String cellName, int row, int column)](#cellNameToIndex-java.lang.String-int-int-) | Hämtar cellens rad- och kolumnindex enligt dess namn |
| [checkCell(int row, int column)](#checkCell-int-int-) | Hämtar [GridCell](../../com.aspose.gridweb/gridcell)-elementet eller null på det angivna cellradindexet och kolumnindexet. |
| [checkColumn(int col)](#checkColumn-int-) | Hämtar [GridColumn](../../com.aspose.gridweb/gridcolumn)-elementet eller null på det angivna kolumnindexet. |
| [checkRow(int i)](#checkRow-int-) | Hämtar [GridRow](../../com.aspose.gridweb/gridrow)-elementet eller null på det angivna cellradindexet. |
| [clear()](#clear--) | Rensa alla celler i samlingen. |
| [clearContents(GridCellArea range)](#clearContents-com.aspose.gridweb.GridCellArea-) | Rensar innehållet i ett intervall. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Rensar innehållet i ett intervall. |
| [clearFormats(GridCellArea range)](#clearFormats-com.aspose.gridweb.GridCellArea-) | Rensar formatering av ett intervall. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Rensar formatering av ett intervall. |
| [clearRange(GridCellArea range)](#clearRange-com.aspose.gridweb.GridCellArea-) | Rensar innehåll och formatering av ett intervall. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Rensar innehåll och formatering av ett intervall. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Hämtar kolumnnamn enligt kolumnindex. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Hämtar kolumnindex enligt kolumnnamn. |
| [copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.gridweb.GridCells-int-int-) | Kopierar data och formatering för en hel kolumn. |
| [copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.gridweb.GridCells-int-int-int-) | Kopierar data och formatering för en hel kolumn. |
| [copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.gridweb.GridCells-int-int-) | Kopierar data och formatering för en hel rad. |
| [copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.gridweb.GridCells-int-int-int-) | Kopierar data och formatering för några hela rader. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Ta bort alla tomma kolumner som inte innehåller någon data. |
| [deleteBlankRows()](#deleteBlankRows--) | Ta bort alla tomma rader som inte innehåller någon data. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Tar bort en kolumn. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Tar bort en kolumn. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Tar bort flera kolumner. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Tar bort ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Tar bort en rad. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Tar bort flera rader. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Tar bort flera rader i kalkylbladet. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Exporterar data i [GridCells](../../com.aspose.gridweb/gridcells)-samlingen till ett tvådimensionellt array‑objekt. |
| [get(int row, int column)](#get-int-int-) | Hämtar [GridCell](../../com.aspose.gridweb/gridcell)-elementet på det angivna cellradindexet och kolumnindexet. |
| [get(String cellName)](#get-java.lang.String-) | Hämtar [GridCell](../../com.aspose.gridweb/gridcell)-elementet på det angivna cellnamnet. |
| [getCell(int row, int column)](#getCell-int-int-) | Hämtar [GridCell](../../com.aspose.gridweb/gridcell)-elementet på det angivna cellradindexet och kolumnindexet. |
| [getClass()](#getClass--) |  |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Hämtar bredden på den angivna kolumnen |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Hämtar bredden på den angivna kolumnen, i tum. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Hämtar bredden på den angivna kolumnen, i pixlar. |
| [getColumns()](#getColumns--) | Hämtar samlingen av [GridColumn](../../com.aspose.gridweb/gridcolumn)-objekt som representerar de enskilda kolumnerna i detta kalkylblad. |
| [getCount()](#getCount--) | Hämtar antalet celler. |
| [getFirstCell()](#getFirstCell--) | Hämtar den första cellen i detta kalkylblad. |
| [getLastCell()](#getLastCell--) | Hämtar den sista cellen i detta kalkylblad. |
| [getMaxColumn()](#getMaxColumn--) | Maximalt kolumnindex för cell som innehåller data eller format. |
| [getMaxDataColumn()](#getMaxDataColumn--) | Maximalt kolumnindex för cellen som innehåller data. |
| [getMaxDataRow()](#getMaxDataRow--) | Maximalt radindex för cellen som innehåller data. |
| [getMaxRow()](#getMaxRow--) | Maximalt radindex för cellen som innehåller data eller stil. |
| [getMergedCells()](#getMergedCells--) | Hämtar samlingen av sammanslagna celler. |
| [getMinColumn()](#getMinColumn--) | Minimalt kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [getMinDataColumn()](#getMinDataColumn--) | Minsta kolumnindex för cell som innehåller data. |
| [getMinDataRow()](#getMinDataRow--) | Minsta radindex för cell som innehåller data. |
| [getMinRow()](#getMinRow--) | Minsta radindex för cell som innehåller data eller stil. |
| [getRow(int i)](#getRow-int-) | Hämtar [GridRow](../../com.aspose.gridweb/gridrow)-elementet eller på det angivna cellradindexet. |
| [getRowEnumerator()](#getRowEnumerator--) | Hämtar enumerator för rader |
| [getRowHeight(int row)](#getRowHeight-int-) | Hämtar höjden på en specificerad rad. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Hämtar höjden på en specificerad rad i enheten tum. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Hämtar höjden på en specificerad rad i enheten pixel. |
| [getRowOutlineLevel(int rowIndex)](#getRowOutlineLevel-int-) | Hämtar konturnivån för raden. |
| [getRows()](#getRows--) | Hämtar samlingen av [GridRow](../../com.aspose.gridweb/gridrow)-objekt som representerar de enskilda raderna i detta kalkylblad. |
| [getStandardHeight()](#getStandardHeight--) | Hämtar standardradens höjd i detta kalkylblad,i enheten punkter. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Hämtar standardradens höjd i detta kalkylblad,i enheten pixlar. |
| [getStandardWidth()](#getStandardWidth--) | Hämtar standardkolumnbredden i kalkylbladet, i tecken. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Hämtar standardkolumnens bredd i kalkylbladet, i enheten tum. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Hämtar standardkolumnens bredd i kalkylbladet, i enheten pixlar. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Hämta bredden i olika vystyper. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Grupperar kolumner. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Grupperar kolumner. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Grupperar rader. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Döljer en kolumn. |
| [hideRow(int row)](#hideRow-int-) | Döljer en rad. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Infogar en ny kolumn i kalkylbladet. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Infogar en ny kolumn i kalkylbladet. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Infogar några kolumner i kalkylbladet. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Infogar några kolumner i kalkylbladet. |
| [insertRange(GridCellArea area, int shiftType)](#insertRange-com.aspose.gridweb.GridCellArea-int-) | Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-) | Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [insertRow(int rowIndex)](#insertRow-int-) | Infogar en ny rad i kalkylbladet. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Infogar flera rader i kalkylbladet. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Infogar flera rader i kalkylbladet. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Kontrollerar om given kolumn är tom (innehåller ingen data). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Kontrollerar om en kolumn på angivet index är dold. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Kontrollerar om en rad på angivet index är dold. |
| [iterator()](#iterator--) | Hämtar enumerator för rader |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Slår ihop ett angivet cellområde till en enda cell. |
| [moveRange(GridCellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.gridweb.GridCellArea-int-int-) | Flyttar området. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Ta bort dubblettvärden i intervallet. |
| [removeFormulas()](#removeFormulas--) | Tar bort alla formler och ersätter dem med formelns värde. |
| [setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)](#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-) | Ställer in kanter för ett cellintervall. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Ställer in bredden på den angivna kolumnen. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Ställer in kolumnbredd i tum. |
| [setColumnWidthPixel(int column, int pixel)](#setColumnWidthPixel-int-int-) | Ställer in kolumnbredd i pixlar. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Ställer in höjden på den angivna raden. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Ställer in radhöjd i tum. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Ställer in radhöjd i pixlar. |
| [setRowOutlineLevel(int rowIndex, int outlineLevel)](#setRowOutlineLevel-int-int-) | Ställer in konturnivån för raden. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Ställer in standardradens höjd i detta kalkylblad,i enheten punkter. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Ställer in standardradens höjd i detta kalkylblad,i enheten pixlar. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Ställer in standardkolumnbredden i kalkylbladet, i tecken. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Ställer in standardkolumnbredden i kalkylbladet, i enheten tum. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Ställer in standardkolumnbredden i kalkylbladet, i enheten pixlar. |
| [setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)](#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-) | Ställer in stilen för ett angivet cellintervall. |
| [setStyle(String cellRange, GridTableItemStyle style)](#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-) | Ställer in stilen för ett angivet cellintervall. |
| [sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)](#sort-int-int-int-int-int-boolean-boolean-boolean-) | Sorterar data stigande/avtagande uppifrån och ner i ett område i ett kalkylblad efter angivet kolumnindex. |
| [sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)](#sort-int-int-int-int-int---int---int-boolean-) | Sorterar data stigande/avtagande uppifrån och ner i ett område i ett kalkylblad efter angivet kolumnindex. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Tar bort sammanslagning av ett angivet område med sammanslagna celler. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Avgrupperar kolumner. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Avgrupperar rader. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Visar en kolumn |
| [unhideRow(int row)](#unhideRow-int-) | Visar en rad. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Hämtar cellnamnet enligt dess rad- och kolumnindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| kolumn | int | Kolumnindex. |

**Returns:**
java.lang.String - Cellens namn.
### cellNameToIndex(String cellName, int row, int column) {#cellNameToIndex-java.lang.String-int-int-}
```
public static void cellNameToIndex(String cellName, int row, int column)
```


Hämtar cellens rad- och kolumnindex enligt dess namn

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellens namn. |
| rad | int | Utdata radindex |
| kolumn | int | Utdata kolumnindex |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public GridCell checkCell(int row, int column)
```


Hämtar [GridCell](../../com.aspose.gridweb/gridcell)-elementet eller null på det angivna cellradindexet och kolumnindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |
| kolumn | int | Kolumnindex |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return GridCell object if a GridCell object exists. Return null if the GridCell does not exist.
### checkColumn(int col) {#checkColumn-int-}
```
public GridColumn checkColumn(int col)
```


Hämtar [GridColumn](../../com.aspose.gridweb/gridcolumn)-elementet eller null på det angivna kolumnindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kol | int | Kolumnindexet. |

**Returns:**
[GridColumn](../../com.aspose.gridweb/gridcolumn) - The Column object.
### checkRow(int i) {#checkRow-int-}
```
public GridRow checkRow(int i)
```


Hämtar [GridRow](../../com.aspose.gridweb/gridrow)-elementet eller null på det angivna cellradindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| i | int | Radindex |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - Returns [GridRow](../../com.aspose.gridweb/gridrow) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Rensa alla celler i samlingen.

### clearContents(GridCellArea range) {#clearContents-com.aspose.gridweb.GridCellArea-}
```
public void clearContents(GridCellArea range)
```


Rensar innehållet i ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Område som ska rensas. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


Rensar innehållet i ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| startColumn | int | Startkolumnens index. |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |

### clearFormats(GridCellArea range) {#clearFormats-com.aspose.gridweb.GridCellArea-}
```
public void clearFormats(GridCellArea range)
```


Rensar formatering av ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Område som ska rensas. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


Rensar formatering av ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| startColumn | int | Startkolumnens index. |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |

### clearRange(GridCellArea range) {#clearRange-com.aspose.gridweb.GridCellArea-}
```
public void clearRange(GridCellArea range)
```


Rensar innehåll och formatering av ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Område som ska rensas. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


Rensar innehåll och formatering av ett intervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| startColumn | int | Startkolumnens index. |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |

### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Hämtar kolumnnamn enligt kolumnindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |

**Returns:**
java.lang.String - Kolumnens namn.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Hämtar kolumnindex enligt kolumnnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnName | java.lang.String | Kolumnnamn. |

**Returns:**
int - Kolumnindex.
### copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.gridweb.GridCells-int-int-}
```
public void copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Kopierar data och formatering för en hel kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Källcellobjektet innehåller data och formatering att kopiera. |
| sourceColumnIndex | int | Källkolumnindex. |
| destinationColumnIndex | int | Destination kolumnindex. |

### copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Kopierar data och formatering för en hel kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Källcellobjektet innehåller data och formatering att kopiera. |
| sourceColumnIndex | int | Källkolumnindex. |
| destinationColumnIndex | int | Destination kolumnindex. |
| columnNumber | int | Det kopierade kolumnnumret. |

### copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.gridweb.GridCells-int-int-}
```
public void copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Kopierar data och formatering för en hel rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Källcellobjektet innehåller data och formatering att kopiera. |
| sourceRowIndex | int | Källradindex. |
| destinationRowIndex | int | Destinationsradindex. |

### copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Kopierar data och formatering för några hela rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | Källcellobjektet innehåller data och formatering att kopiera. |
| sourceRowIndex | int | Källradindex. |
| destinationRowIndex | int | Destinationsradindex. |
| rowNumber | int | Det kopierade radnumret. |

### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Ta bort alla tomma kolumner som inte innehåller någon data.

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Ta bort alla tomma rader som inte innehåller någon data.

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Tar bort en kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Tar bort en kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| updateReference | boolean | Indikerar om referenser i andra kalkylblad ska uppdateras. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Tar bort flera kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| totalColumns | int | Antal kolumner som ska tas bort. |
| updateReference | boolean | Indikerar om referenser i andra kalkylblad ska uppdateras. |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


Tar bort ett cellområde och flyttar celler enligt förskjutningsalternativet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| startColumn | int | Startkolumnens index. |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Skiftcellalternativ. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Tar bort en rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Tar bort flera rader.

**Remarks**

Om det borttagna intervallet innehåller den övre delen (inte hela) av tabellen (ListObject) kan intervallet inte tas bort och inget görs. Det fungerar som i MS Excel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Det första radindexet som ska raderas. |
| totalRows | int | Antal rader som ska tas bort. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


Tar bort flera rader i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |
| totalRows | int | Antal rader som ska tas bort. |
| updateReference | boolean | Indikerar om referenser i andra kalkylblad ska uppdateras. |

**Returns:**
boolean -
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
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Exporterar data i [GridCells](../../com.aspose.gridweb/gridcells)-samlingen till ett tvådimensionellt array‑objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Radnumret för den första cellen som ska exporteras. |
| firstColumn | int | Kolumnnumret för den första cellen som ska exporteras. |
| totalRows | int | Antal rader att exportera |
| totalColumns | int | Antal kolumner att exportera |

**Returns:**
java.lang.Object[][] - Exporterat cellvärdesmatrisobjekt.
### get(int row, int column) {#get-int-int-}
```
public GridCell get(int row, int column)
```


Hämtar [GridCell](../../com.aspose.gridweb/gridcell)-elementet på det angivna cellradindexet och kolumnindexet.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
         //Gets the cell at "A1"
         GridCell cell = cells.get(0, 0);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| kolumn | int | Kolumnindex. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The [GridCell](../../com.aspose.gridweb/gridcell) object.
### get(String cellName) {#get-java.lang.String-}
```
public GridCell get(String cellName)
```


Hämtar [GridCell](../../com.aspose.gridweb/gridcell)-elementet på det angivna cellnamnet.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
          GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
          GridCell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn, inklusive dess kolumnbokstav och radnummer, till exempel A5. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - A [GridCell](../../com.aspose.gridweb/gridcell) object
### getCell(int row, int column) {#getCell-int-int-}
```
public GridCell getCell(int row, int column)
```


Hämtar [GridCell](../../com.aspose.gridweb/gridcell)-elementet på det angivna cellradindexet och kolumnindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |
| kolumn | int | Kolumnindex |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return Cell object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Hämtar bredden på den angivna kolumnen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex |

**Returns:**
double - Kolumnbredd
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Hämtar bredden på den angivna kolumnen, i tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex |

**Returns:**
double - Kolumnbredd
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Hämtar bredden på den angivna kolumnen, i pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex |

**Returns:**
int – Kolumnens bredd i normal vy.
### getColumns() {#getColumns--}
```
public GridColumnCollection getColumns()
```


Hämtar samlingen av [GridColumn](../../com.aspose.gridweb/gridcolumn)-objekt som representerar de enskilda kolumnerna i detta kalkylblad.

**Returns:**
[GridColumnCollection](../../com.aspose.gridweb/gridcolumncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Hämtar antalet celler.

**Returns:**
int
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Hämtar den första cellen i detta kalkylblad.

**Remarks**

Returnerar null om det inte finns någon data i kalkylbladet.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Hämtar den sista cellen i detta kalkylblad.

**Remarks**

Returnerar null om det inte finns någon data i kalkylbladet.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Maximalt kolumnindex för cell som innehåller data eller format.

**Remarks**

Returnera -1 om det inte finns någon cell.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Maximalt kolumnindex för cellen som innehåller data.

**Remarks**

\-1 kommer att returneras om det inte finns någon cell som innehåller data. Denna egenskap måste iterera och kontrollera alla celler i ett kalkylblad, så det är en tidskrävande process och bör inte anropas upprepade gånger.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Maximalt radindex för cellen som innehåller data.

**Remarks**

Returnera -1 om det inte finns någon cell som innehåller data.

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Maximalt radindex för cellen som innehåller data eller stil.

**Remarks**

Returnera -1 om det inte finns någon cell som innehåller data eller stil i kalkylbladet.

**Returns:**
int
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Hämtar samlingen av sammanslagna celler.

**Remarks**

I den här samlingen är varje objekt en [GridCellArea](../../com.aspose.gridweb/gridcellarea) struktur som representerar ett område av sammanslagna celler.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Minimalt kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den).

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Minsta kolumnindex för cell som innehåller data.

**Remarks**

\-1 kommer att returneras om det inte finns någon cell som innehåller data. Denna egenskap måste iterera och kontrollera alla celler i ett kalkylblad, så det är en tidskrävande process och bör inte anropas upprepade gånger.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Minsta radindex för cell som innehåller data.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Minsta radindex för cell som innehåller data eller stil.

**Returns:**
int
### getRow(int i) {#getRow-int-}
```
public GridRow getRow(int i)
```


Hämtar [GridRow](../../com.aspose.gridweb/gridrow)-elementet eller på det angivna cellradindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| i | int | Radindex |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - the row object
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Hämtar enumerator för rader

**Returns:**
java.util.Iterator - Radernas iterator.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Hämtar höjden på en specificerad rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |

**Returns:**
double - Radhöjd
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


Hämtar höjden på en specificerad rad i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |

**Returns:**
double - Radhöjd
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


Hämtar höjden på en specificerad rad i enheten pixel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex |

**Returns:**
int - Radhöjd
### getRowOutlineLevel(int rowIndex) {#getRowOutlineLevel-int-}
```
public int getRowOutlineLevel(int rowIndex)
```


Hämtar konturnivån för raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | radindex. |

**Returns:**
int - konturnivån.
### getRows() {#getRows--}
```
public GridRowCollection getRows()
```


Hämtar samlingen av [GridRow](../../com.aspose.gridweb/gridrow)-objekt som representerar de enskilda raderna i detta kalkylblad.

**Returns:**
[GridRowCollection](../../com.aspose.gridweb/gridrowcollection)
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
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Hämtar standardkolumnbredden i kalkylbladet, i tecken.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


Hämtar standardkolumnens bredd i kalkylbladet, i enheten tum.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


Hämtar standardkolumnens bredd i kalkylbladet, i enheten pixlar.

**Returns:**
int
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


Hämta bredden i olika vystyper.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindexet. |

**Returns:**
int - kolumnbredd i enhet av pixlar
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


Grupperar kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första kolumnindexet som ska grupperas. |
| lastIndex | int | Det sista kolumnindexet som ska grupperas. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


Grupperar kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första kolumnindexet som ska grupperas. |
| lastIndex | int | Det sista kolumnindexet som ska grupperas. |
| isHidden | boolean | Anger om de grupperade kolumnerna är dolda. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Grupperar rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska grupperas. |
| lastIndex | int | Det sista radindexet som ska grupperas. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```


Döljer en kolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Döljer en rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


Infogar en ny kolumn i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


Infogar en ny kolumn i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| updateReference | boolean | Indikerar om referenser i andra arbetsblad kommer att uppdateras. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


Infogar några kolumner i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| totalColumns | int | Antalet kolumner. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Infogar några kolumner i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| totalColumns | int | Antalet kolumner. |
| updateReference | boolean | Indikerar om referenser i andra arbetsblad kommer att uppdateras. |

### insertRange(GridCellArea area, int shiftType) {#insertRange-com.aspose.gridweb.GridCellArea-int-}
```
public void insertRange(GridCellArea area, int shiftType)
```


Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Flyttområde. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Skiftcellalternativ. |

### insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-}
```
public void insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Flyttområde. |
| shiftNumber | int | Antal rader eller kolumner som ska infogas. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Skiftcellalternativ. |
| updateReference | boolean | Indikerar om referenser i andra kalkylblad ska uppdateras. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


Infogar en ny rad i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


Infogar flera rader i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |
| totalRows | int | Antal rader som ska infogas. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


Infogar flera rader i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |
| totalRows | int | Antal rader som ska infogas. |
| updateReference | boolean | Indikerar om referenser i andra arbetsblad kommer att uppdateras. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


Kontrollerar om given kolumn är tom (innehåller ingen data).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | kolumnindexet |

**Returns:**
boolesk - true om given kolumn inte innehåller någon data
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


Kontrollerar om en kolumn på angivet index är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | kolumnindex |

**Returns:**
boolesk - true om kolumnen är dold.
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


Kontrollerar om en rad på angivet index är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | radindex |

**Returns:**
boolesk - true om raden är dold
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hämtar enumerator för rader

**Returns:**
java.util.Iterator - Enumeratör för rader
### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Slår ihop ett angivet cellområde till en enda cell.

**Remarks**

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i intervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första raden i detta intervall (nollbaserat) |
| firstColumn | int | Första kolumnen i detta intervall (nollbaserat) |
| totalRows | int | Antal rader (enbaserat) |
| totalColumns | int | Antal kolumner (enbaserat) |

### moveRange(GridCellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.gridweb.GridCellArea-int-int-}
```
public void moveRange(GridCellArea sourceArea, int destRow, int destColumn)
```


Flyttar området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Det område som ska flyttas. |
| destRow | int | Målraden. |
| destColumn | int | Målkolumnen. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Ta bort dubblettvärden i intervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startrad. |
| startColumn | int | Startkolumn |
| slutRad | int | Slutradens index. |
| endColumn | int | Slutkolumnens index. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Tar bort alla formler och ersätter dem med formelns värde.

### setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle) {#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)
```


Ställer in kanter för ett cellintervall.

**Example**

```
           GridWeb GridWeb1 = new GridWeb();
           WebBorderStyle borderStyle1 = new WebBorderStyle();
         	 GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, borderStyle1);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Det första radnumret i intervallet (nollbaserat). |
| firstColumn | int | Det första kolumnnumret i intervallet (nollbaserat). |
| rowNumber | int | Antalet rader. |
| columnNumber | int | Antalet kolumner. |
| position | int | [SetBorderPosition](../../com.aspose.gridweb/setborderposition). Kantpositionen. |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Kantstilen. |

### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Ställer in bredden på den angivna kolumnen.

**Remarks**

För att dölja en kolumn, sätt kolumnbredden till noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| bredd | double | Kolumnbredd. Kolumnbredden måste vara mellan 0 och 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Ställer in kolumnbredd i tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| tum | double | Antal tum. |

### setColumnWidthPixel(int column, int pixel) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixel)
```


Ställer in kolumnbredd i pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| pixel | int | Antal pixlar. |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Ställer in höjden på den angivna raden.

**Remarks**

För att dölja en rad, sätt radhöjden till noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| höjd | double | Radhöjd i punktenheter. Den bör vara mellan 0 och 409,5. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


Ställer in radhöjd i tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| tum | double | Antal tum. Det bör vara mellan 0 och 409,5/72. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


Ställer in radhöjd i pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| pixlar | int | Antal pixlar. |

### setRowOutlineLevel(int rowIndex, int outlineLevel) {#setRowOutlineLevel-int-int-}
```
public void setRowOutlineLevel(int rowIndex, int outlineLevel)
```


Ställer in konturnivån för raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | radindex. |
| outlineLevel | int | konturnivå. |

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

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Ställer in standardkolumnbredden i kalkylbladet, i tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


Ställer in standardkolumnbredden i kalkylbladet, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


Ställer in standardkolumnbredden i kalkylbladet, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style) {#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)
```


Ställer in stilen för ett angivet cellintervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första raden i detta intervall (nollbaserat) |
| firstColumn | int | Första kolumnen i detta intervall (nollbaserat) |
| rowNumber | int | Antal rader (enbaserat) |
| columnNumber | int | Antal kolumner (enbaserat) |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Stilobjektet som ska sättas |

### setStyle(String cellRange, GridTableItemStyle style) {#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(String cellRange, GridTableItemStyle style)
```


Ställer in stilen för ett angivet cellintervall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellRange | java.lang.String | Intervallet av cellnamn, t.ex. "A1:D6" |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Stilobjektet som ska sättas |

### sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright) {#sort-int-int-int-int-int-boolean-boolean-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)
```


Sorterar data stigande/avtagande uppifrån och ner i ett område av ett kalkylblad efter angivet kolumnindex. Sorterar data stigande/avtagande från vänster till höger i ett område av ett kalkylblad efter angivet radindex.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWeb1.getWorkSheets().get(0).getCells().sort(1,0,25,6,3,true,true,false);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Radnumret för den första cellen som ska sorteras. |
| startColumn | int | Kolumnnumret för den första cellen att sortera. |
| rader | int | Antal rader som ska importeras. |
| kolumner | int | Antal kolumner som ska importeras. |
| index | int | Kolumnindex som specificerar sorteringskolumnen. om Orienteringen är uppifrån och ner, står den för kolumnindex som specificerar sorteringskolumnen. om Orienteringen är från vänster till höger, står den för radindex som specificerar sorteringsraden. |
| isAsending | boolean | om sorteringsordningen är stigande. |
| isCaseSensitive | boolean | om sorteringen är skiftlägeskänslig. |
| islefttoright | boolean | om sorteringsorienteringen är från vänster till höger |

### sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive) {#sort-int-int-int-int-int---int---int-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)
```


Sorterar data stigande/avtagande uppifrån och ner i ett område av ett kalkylblad efter angivet kolumnindex. Sorterar data stigande/avtagande från vänster till höger i ett område av ett kalkylblad efter angivet radindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Radnumret för den första cellen som ska sorteras. |
| startColumn | int | Kolumnnumret för den första cellen att sortera. |
| rader | int | Antal rader som ska importeras. |
| kolumner | int | Antal kolumner som ska importeras. |
| index | int[] | Kolumnindexarray som specificerar sorteringskolumnen. om Orienteringen är uppifrån och ner, står den för kolumnindex som specificerar sorteringskolumnen. om Orienteringen är från vänster till höger, står den för radindex som specificerar sorteringsraden. |
| orders | int[] | [SortByOrder](../../com.aspose.gridweb/sortbyorder). sorteringsordningsarrayen. |
| orientation | int | [SortOrientation](../../com.aspose.gridweb/sortorientation). sorteringsorientering |
| isCaseSensitive | boolean | om sorteringen är skiftlägeskänslig. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#unMerge-int-int-int-int-}
```
public void unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Tar bort sammanslagning av ett angivet område med sammanslagna celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första raden i detta intervall (nollbaserat) |
| firstColumn | int | Första kolumnen i detta intervall (nollbaserat) |
| totalRows | int | Antal rader (enbaserat) |
| totalColumns | int | Antal kolumner (enbaserat) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


Avgrupperar kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första kolumnindexet som ska avgrupperas. |
| lastIndex | int | Det sista kolumnindexet som ska avgrupperas. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Avgrupperar rader.

**Remarks**

Tar bara bort yttre gruppinformation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska avgrupperas. |
| lastIndex | int | Det sista radindexet som ska avgrupperas. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Visar en kolumn

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindex. |
| bredd | double | Kolumnbredd..Kolumnbredd måste vara mellan 0 och 255 |

### unhideRow(int row) {#unhideRow-int-}
```
public void unhideRow(int row)
```


Visar en rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |

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

