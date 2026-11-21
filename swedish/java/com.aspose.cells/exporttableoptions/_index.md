---
title: "ExportTableOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla exporttabellalternativ."
type: docs
url: /sv/java/com.aspose.cells/exporttableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ExportTableOptions
```

Representerar alla exporttabellalternativ.

**Remarks**

Om det finns några speciella krav på exporten, såsom att ignorera felvärden, kan användaren utöka den här klassen för att skriva över motsvarande API:er för att uppnå målet.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [ExportTableOptions()](#ExportTableOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDBNull()](#getAllowDBNull--) | Detta värde indikerar om DBNulls är tillåtna i den här tabellen. |
| [getCheckMixedValueType()](#getCheckMixedValueType--) | Falskt, Aspose.Cells kommer att sätta DataColumn:s typ baserat på värdetypen för den första raden för prestanda. |
| [getClass()](#getClass--) |  |
| [getExportAsHtmlString()](#getExportAsHtmlString--) | Exporterar cellernas HTML-strängvärde till DataTable. |
| [getExportAsString()](#getExportAsString--) | Exporterar cellernas strängvärde till DataTable. |
| [getExportColumnName()](#getExportColumnName--) | Indikerar om data i den första raden exporteras till kolumnnamnet i DataTable. |
| [getFormatStrategy()](#getFormatStrategy--) | Hämtar formatstrategin när värdet exporteras som strängvärde. |
| [getIndexes()](#getIndexes--) | Indexen för kolumner/rader som ska exporteras. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Exporterar endast synliga celler. |
| [getPlotVisibleColumns()](#getPlotVisibleColumns--) | Exporterar endast synliga kolumner. |
| [getPlotVisibleRows()](#getPlotVisibleRows--) | Exporterar endast synliga rader. |
| [getRenameStrategy()](#getRenameStrategy--) | Strategi för dubblettnamn på kolumner. |
| [getSkipErrorValue()](#getSkipErrorValue--) | Indikerar om ogiltiga värden ska hoppas över för kolumnen. |
| [hashCode()](#hashCode--) |  |
| [isVertical()](#isVertical--) | Sant om en rad i Workbook-filen representerar en rad i DataTable. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [preprocessExportedValue(int cellRow, int cellColumn, CellValue value)](#preprocessExportedValue-int-int-com.aspose.cells.CellValue-) | Förbehandla värdet i den aktuella cellen som ska exporteras. |
| [setAllowDBNull(boolean value)](#setAllowDBNull-boolean-) | Detta värde indikerar om DBNulls är tillåtna i den här tabellen. |
| [setCheckMixedValueType(boolean value)](#setCheckMixedValueType-boolean-) | Falskt, Aspose.Cells kommer att sätta DataColumn:s typ baserat på värdetypen för den första raden för prestanda. |
| [setExportAsHtmlString(boolean value)](#setExportAsHtmlString-boolean-) | Exporterar cellernas HTML-strängvärde till DataTable. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Exporterar cellernas strängvärde till DataTable. |
| [setExportColumnName(boolean value)](#setExportColumnName-boolean-) | Indikerar om data i den första raden exporteras till kolumnnamnet i DataTable. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Ställer in formatstrategin när värdet exporteras som strängvärde. |
| [setIndexes(int[] value)](#setIndexes-int---) | Indexen för kolumner/rader som ska exporteras. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Exporterar endast synliga celler. |
| [setPlotVisibleColumns(boolean value)](#setPlotVisibleColumns-boolean-) | Exporterar endast synliga kolumner. |
| [setPlotVisibleRows(boolean value)](#setPlotVisibleRows-boolean-) | Exporterar endast synliga rader. |
| [setRenameStrategy(int value)](#setRenameStrategy-int-) | Strategi för dubblettnamn på kolumner. |
| [setSkipErrorValue(boolean value)](#setSkipErrorValue-boolean-) | Indikerar om ogiltiga värden ska hoppas över för kolumnen. |
| [setVertical(boolean value)](#setVertical-boolean-) | Sant om en rad i Workbook-filen representerar en rad i DataTable. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ExportTableOptions() {#ExportTableOptions--}
```
public ExportTableOptions()
```


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
### getAllowDBNull() {#getAllowDBNull--}
```
public boolean getAllowDBNull()
```


Detta värde indikerar om DBNulls är tillåtna i den här tabellen.

**Returns:**
boolean
### getCheckMixedValueType() {#getCheckMixedValueType--}
```
public boolean getCheckMixedValueType()
```


Falskt, Aspose.Cells kommer att sätta DataColumn's type efter värdetypen i den första raden för prestanda. Sant, Aspose.Cells kommer att kontrollera om värdetypen i kolumnen är blandad innan DataColumn's type sätts. Om värdetypen är blandad, blir DataColumn's type string.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExportAsHtmlString() {#getExportAsHtmlString--}
```
public boolean getExportAsHtmlString()
```


Exporterar cellernas HTML-strängvärde till DataTable.

**Returns:**
boolean
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Exporterar cellernas strängvärde till DataTable.

**Returns:**
boolean
### getExportColumnName() {#getExportColumnName--}
```
public boolean getExportColumnName()
```


Anger om data i den första raden exporteras till kolumnnamnet i DataTable. Standardvärdet är falskt.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Hämtar formatstrategin när värdet exporteras som strängvärde.

Se [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Standardvärdet är [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Returns:**
int
### getIndexes() {#getIndexes--}
```
public int[] getIndexes()
```


Indexen för kolumner/rader som ska exporteras.

**Returns:**
int[]
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Exporterar endast synliga celler.

**Returns:**
boolean
### getPlotVisibleColumns() {#getPlotVisibleColumns--}
```
public boolean getPlotVisibleColumns()
```


Exporterar endast synliga kolumner.

**Returns:**
boolean
### getPlotVisibleRows() {#getPlotVisibleRows--}
```
public boolean getPlotVisibleRows()
```


Exporterar endast synliga rader.

**Returns:**
boolean
### getRenameStrategy() {#getRenameStrategy--}
```
public int getRenameStrategy()
```


Strategi för dubblettnamn på kolumner.

Se [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Returns:**
int
### getSkipErrorValue() {#getSkipErrorValue--}
```
public boolean getSkipErrorValue()
```


Anger om ogiltiga värden för kolumnen ska hoppas över. Till exempel, om kolumntypen är decimal, värdet är större än decimal.MaxValue och denna egenskap är sann, kommer vi inte att kasta ett undantag igen. Standardvärdet är falskt.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVertical() {#isVertical--}
```
public boolean isVertical()
```


Sant om en rad i Workbook-filen representerar en rad i DataTable. Falskt om en kolumn i Workbook-filen representerar en rad i DataTable.

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




### preprocessExportedValue(int cellRow, int cellColumn, CellValue value) {#preprocessExportedValue-int-int-com.aspose.cells.CellValue-}
```
public boolean preprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```


Förbehandla värdet i den aktuella cellen som ska exporteras.

**Remarks**

Rad- och kolumnindexet är cellens absoluta index i kalkylbladet, inte indexet i den exporterade tabellen. Användaren kan kontrollera värdet i den aktuella cellen i den överskrivna implementeringen av denna metod; om den aktuella cellen behöver ersättas med en annan typ och värde, bör implementeringen sätta den förväntade typen och värdet i CellValue-objektet och returnera true. Som standard gör denna metod ingenting och returnerar false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellRow | int | radindexet för den aktuella cellen |
| cellColumn | int | kolumnindexet för cellen |
| value | [CellValue](../../com.aspose.cells/cellvalue) | värde och typ för den aktuella cellen |

**Returns:**
boolesk - Om den aktuella cellen har ersatts med en annan typ och/eller värde.
### setAllowDBNull(boolean value) {#setAllowDBNull-boolean-}
```
public void setAllowDBNull(boolean value)
```


Detta värde indikerar om DBNulls är tillåtna i den här tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCheckMixedValueType(boolean value) {#setCheckMixedValueType-boolean-}
```
public void setCheckMixedValueType(boolean value)
```


Falskt, Aspose.Cells kommer att sätta DataColumn's type efter värdetypen i den första raden för prestanda. Sant, Aspose.Cells kommer att kontrollera om värdetypen i kolumnen är blandad innan DataColumn's type sätts. Om värdetypen är blandad, blir DataColumn's type string.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportAsHtmlString(boolean value) {#setExportAsHtmlString-boolean-}
```
public void setExportAsHtmlString(boolean value)
```


Exporterar cellernas HTML-strängvärde till DataTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Exporterar cellernas strängvärde till DataTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportColumnName(boolean value) {#setExportColumnName-boolean-}
```
public void setExportColumnName(boolean value)
```


Anger om data i den första raden exporteras till kolumnnamnet i DataTable. Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Ställer in formatstrategin när värdet exporteras som strängvärde.

Se [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Standardvärdet är [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setIndexes(int[] value) {#setIndexes-int---}
```
public void setIndexes(int[] value)
```


Indexen för kolumner/rader som ska exporteras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int[] |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Exporterar endast synliga celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPlotVisibleColumns(boolean value) {#setPlotVisibleColumns-boolean-}
```
public void setPlotVisibleColumns(boolean value)
```


Exporterar endast synliga kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPlotVisibleRows(boolean value) {#setPlotVisibleRows-boolean-}
```
public void setPlotVisibleRows(boolean value)
```


Exporterar endast synliga rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRenameStrategy(int value) {#setRenameStrategy-int-}
```
public void setRenameStrategy(int value)
```


Strategi för dubblettnamn på kolumner.

Se [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSkipErrorValue(boolean value) {#setSkipErrorValue-boolean-}
```
public void setSkipErrorValue(boolean value)
```


Anger om ogiltiga värden för kolumnen ska hoppas över. Till exempel, om kolumntypen är decimal, värdet är större än decimal.MaxValue och denna egenskap är sann, kommer vi inte att kasta ett undantag igen. Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setVertical(boolean value) {#setVertical-boolean-}
```
public void setVertical(boolean value)
```


Sant om en rad i Workbook-filen representerar en rad i DataTable. Falskt om en kolumn i Workbook-filen representerar en rad i DataTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

