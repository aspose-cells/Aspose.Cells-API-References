---
title: ExportTableOptions
second_title: Aspose.Cells for Java API Reference
description: Represents all export table options.
type: docs
weight: 200
url: /java/com.aspose.cells/exporttableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ExportTableOptions
```

Represents all export table options.
## Constructors

| Constructor | Description |
| --- | --- |
| [ExportTableOptions()](#ExportTableOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckMixedValueType()](#getCheckMixedValueType--) | False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance. |
| [getClass()](#getClass--) |  |
| [getExportAsHtmlString()](#getExportAsHtmlString--) | Exports the html string value of the cells to the DataTable. |
| [getExportAsString()](#getExportAsString--) | Exports the string value of the cells to the DataTable. |
| [getExportColumnName()](#getExportColumnName--) | Indicates whether the data in the first row are exported to the column name of the DataTable. |
| [getFormatStrategy()](#getFormatStrategy--) | the format strategy when exporting the value as string value. |
| [getIndexes()](#getIndexes--) | The indexes of columns/rows which should be exported out. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Only exports visible cells. |
| [getPlotVisibleColumns()](#getPlotVisibleColumns--) | Only exports visible columns. |
| [getPlotVisibleRows()](#getPlotVisibleRows--) | Only exports visible rows. |
| [getRenameStrategy()](#getRenameStrategy--) | Strategy for duplicate names of columns. |
| [getSkipErrorValue()](#getSkipErrorValue--) | Indicates whether skip invalid value for the column. |
| [hashCode()](#hashCode--) |  |
| [isVertical()](#isVertical--) | True if a row in Workbook file represents a row in DataTable. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMixedValueType(boolean value)](#setCheckMixedValueType-boolean-) | For the description of this property, please see [getCheckMixedValueType()](../../com.aspose.cells/exporttableoptions\#getCheckMixedValueType--) |
| [setExportAsHtmlString(boolean value)](#setExportAsHtmlString-boolean-) | For the description of this property, please see [getExportAsHtmlString()](../../com.aspose.cells/exporttableoptions\#getExportAsHtmlString--) |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | For the description of this property, please see [getExportAsString()](../../com.aspose.cells/exporttableoptions\#getExportAsString--) |
| [setExportColumnName(boolean value)](#setExportColumnName-boolean-) | For the description of this property, please see [getExportColumnName()](../../com.aspose.cells/exporttableoptions\#getExportColumnName--) |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | For the description of this property, please see [getFormatStrategy()](../../com.aspose.cells/exporttableoptions\#getFormatStrategy--) |
| [setIndexes(int[] value)](#setIndexes-int---) | For the description of this property, please see [getIndexes()](../../com.aspose.cells/exporttableoptions\#getIndexes--) |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | For the description of this property, please see [getPlotVisibleCells()](../../com.aspose.cells/exporttableoptions\#getPlotVisibleCells--) |
| [setPlotVisibleColumns(boolean value)](#setPlotVisibleColumns-boolean-) | For the description of this property, please see [getPlotVisibleColumns()](../../com.aspose.cells/exporttableoptions\#getPlotVisibleColumns--) |
| [setPlotVisibleRows(boolean value)](#setPlotVisibleRows-boolean-) | For the description of this property, please see [getPlotVisibleRows()](../../com.aspose.cells/exporttableoptions\#getPlotVisibleRows--) |
| [setRenameStrategy(int value)](#setRenameStrategy-int-) | For the description of this property, please see [getRenameStrategy()](../../com.aspose.cells/exporttableoptions\#getRenameStrategy--) |
| [setSkipErrorValue(boolean value)](#setSkipErrorValue-boolean-) | For the description of this property, please see [getSkipErrorValue()](../../com.aspose.cells/exporttableoptions\#getSkipErrorValue--) |
| [setVertical(boolean value)](#setVertical-boolean-) | For the description of this property, please see [isVertical()](../../com.aspose.cells/exporttableoptions\#isVertical--) |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCheckMixedValueType() {#getCheckMixedValueType--}
```
public boolean getCheckMixedValueType()
```


False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance. True, Aspose.Cells will check whether the value type in the column are mixed before set the DataColumn's type And the value type are mixed, the DataColumn's type will be string.

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


Exports the html string value of the cells to the DataTable.

**Returns:**
boolean
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Exports the string value of the cells to the DataTable.

**Returns:**
boolean
### getExportColumnName() {#getExportColumnName--}
```
public boolean getExportColumnName()
```


Indicates whether the data in the first row are exported to the column name of the DataTable. The default value is false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


the format strategy when exporting the value as string value.

**Returns:**
int
### getIndexes() {#getIndexes--}
```
public int[] getIndexes()
```


The indexes of columns/rows which should be exported out.

**Returns:**
int[]
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Only exports visible cells.

**Returns:**
boolean
### getPlotVisibleColumns() {#getPlotVisibleColumns--}
```
public boolean getPlotVisibleColumns()
```


Only exports visible columns.

**Returns:**
boolean
### getPlotVisibleRows() {#getPlotVisibleRows--}
```
public boolean getPlotVisibleRows()
```


Only exports visible rows.

**Returns:**
boolean
### getRenameStrategy() {#getRenameStrategy--}
```
public int getRenameStrategy()
```


Strategy for duplicate names of columns.

**Returns:**
int
### getSkipErrorValue() {#getSkipErrorValue--}
```
public boolean getSkipErrorValue()
```


Indicates whether skip invalid value for the column. For example,if the column type is decimal ,the value is greater than decimal.MaxValue and this property is true,we will not throw exception again. The default value is false.

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


True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable.

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




### setCheckMixedValueType(boolean value) {#setCheckMixedValueType-boolean-}
```
public void setCheckMixedValueType(boolean value)
```


For the description of this property, please see [getCheckMixedValueType()](../../com.aspose.cells/exporttableoptions\#getCheckMixedValueType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportAsHtmlString(boolean value) {#setExportAsHtmlString-boolean-}
```
public void setExportAsHtmlString(boolean value)
```


For the description of this property, please see [getExportAsHtmlString()](../../com.aspose.cells/exporttableoptions\#getExportAsHtmlString--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


For the description of this property, please see [getExportAsString()](../../com.aspose.cells/exporttableoptions\#getExportAsString--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportColumnName(boolean value) {#setExportColumnName-boolean-}
```
public void setExportColumnName(boolean value)
```


For the description of this property, please see [getExportColumnName()](../../com.aspose.cells/exporttableoptions\#getExportColumnName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


For the description of this property, please see [getFormatStrategy()](../../com.aspose.cells/exporttableoptions\#getFormatStrategy--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setIndexes(int[] value) {#setIndexes-int---}
```
public void setIndexes(int[] value)
```


For the description of this property, please see [getIndexes()](../../com.aspose.cells/exporttableoptions\#getIndexes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int[] |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


For the description of this property, please see [getPlotVisibleCells()](../../com.aspose.cells/exporttableoptions\#getPlotVisibleCells--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPlotVisibleColumns(boolean value) {#setPlotVisibleColumns-boolean-}
```
public void setPlotVisibleColumns(boolean value)
```


For the description of this property, please see [getPlotVisibleColumns()](../../com.aspose.cells/exporttableoptions\#getPlotVisibleColumns--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPlotVisibleRows(boolean value) {#setPlotVisibleRows-boolean-}
```
public void setPlotVisibleRows(boolean value)
```


For the description of this property, please see [getPlotVisibleRows()](../../com.aspose.cells/exporttableoptions\#getPlotVisibleRows--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRenameStrategy(int value) {#setRenameStrategy-int-}
```
public void setRenameStrategy(int value)
```


For the description of this property, please see [getRenameStrategy()](../../com.aspose.cells/exporttableoptions\#getRenameStrategy--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSkipErrorValue(boolean value) {#setSkipErrorValue-boolean-}
```
public void setSkipErrorValue(boolean value)
```


For the description of this property, please see [getSkipErrorValue()](../../com.aspose.cells/exporttableoptions\#getSkipErrorValue--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setVertical(boolean value) {#setVertical-boolean-}
```
public void setVertical(boolean value)
```


For the description of this property, please see [isVertical()](../../com.aspose.cells/exporttableoptions\#isVertical--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

