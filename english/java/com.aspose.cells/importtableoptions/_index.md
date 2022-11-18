---
title: ImportTableOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options of importing data into cells.
type: docs
weight: 276
url: /java/com.aspose.cells/importtableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImportTableOptions
```

Represents the options of importing data into cells.
## Constructors

| Constructor | Description |
| --- | --- |
| [ImportTableOptions()](#ImportTableOptions--) | Creates the default importing options. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckMergedCells()](#getCheckMergedCells--) | Indicates whether checking merged cells. |
| [getClass()](#getClass--) |  |
| [getColumnIndexes()](#getColumnIndexes--) | Gets or sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [getConvertGridStyle()](#getConvertGridStyle--) | Indicates whether apply the style of the grid view to cells. |
| [getConvertNumericData()](#getConvertNumericData--) | Gets or sets a value that indicates whether the string value should be converted to numeric or date value. |
| [getDateFormat()](#getDateFormat--) | Gets or sets date format string for cells with imported datetime values. |
| [getDefaultValues()](#getDefaultValues--) | Default value for the value in the table is null. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--) | Indicates whether exporting caption as field name Only works for DataTable. |
| [getInsertRows()](#getInsertRows--) | Indicates whether new rows should be added for importing data records. |
| [getNumberFormats()](#getNumberFormats--) | Gets or sets the number formats |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--) | Indicates whether shifting the first row down when inserting rows. |
| [getTotalColumns()](#getTotalColumns--) | Gets or sets total column count to import from data source. -1 means all rows of given data source. |
| [getTotalRows()](#getTotalRows--) | Gets or sets total row count to import from data source. -1 means all rows of given data source. |
| [hashCode()](#hashCode--) |  |
| [isFieldNameShown()](#isFieldNameShown--) | Indicates whether field name should be imported. |
| [isFormulas()](#isFormulas--) | Indicates whether the data are formulas. |
| [isHtmlString()](#isHtmlString--) | Indicates whether the value contains html tags. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMergedCells(boolean value)](#setCheckMergedCells-boolean-) | For the description of this property, please see \#getCheckMergedCells().getCheckMergedCells() |
| [setColumnIndexes(int[] value)](#setColumnIndexes-int---) | For the description of this property, please see \#getColumnIndexes().getColumnIndexes() |
| [setConvertGridStyle(boolean value)](#setConvertGridStyle-boolean-) | For the description of this property, please see \#getConvertGridStyle().getConvertGridStyle() |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | For the description of this property, please see \#getConvertNumericData().getConvertNumericData() |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | For the description of this property, please see \#getDateFormat().getDateFormat() |
| [setDefaultValues(Object[] value)](#setDefaultValues-java.lang.Object---) | For the description of this property, please see \#getDefaultValues().getDefaultValues() |
| [setExportCaptionAsFieldName(boolean value)](#setExportCaptionAsFieldName-boolean-) | For the description of this property, please see \#getExportCaptionAsFieldName().getExportCaptionAsFieldName() |
| [setFieldNameShown(boolean value)](#setFieldNameShown-boolean-) | For the description of this property, please see \#isFieldNameShown().isFieldNameShown() |
| [setFormulas(boolean[] value)](#setFormulas-boolean---) | For the description of this property, please see \#isFormulas().isFormulas() |
| [setHtmlString(boolean value)](#setHtmlString-boolean-) | For the description of this property, please see \#isHtmlString().isHtmlString() |
| [setInsertRows(boolean value)](#setInsertRows-boolean-) | For the description of this property, please see \#getInsertRows().getInsertRows() |
| [setNumberFormats(String[] value)](#setNumberFormats-java.lang.String---) | For the description of this property, please see \#getNumberFormats().getNumberFormats() |
| [setShiftFirstRowDown(boolean value)](#setShiftFirstRowDown-boolean-) | For the description of this property, please see \#getShiftFirstRowDown().getShiftFirstRowDown() |
| [setTotalColumns(int value)](#setTotalColumns-int-) | For the description of this property, please see \#getTotalColumns().getTotalColumns() |
| [setTotalRows(int value)](#setTotalRows-int-) | For the description of this property, please see \#getTotalRows().getTotalRows() |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImportTableOptions() {#ImportTableOptions--}
```
public ImportTableOptions()
```


Creates the default importing options.

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
### getCheckMergedCells() {#getCheckMergedCells--}
```
public boolean getCheckMergedCells()
```


Indicates whether checking merged cells.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnIndexes() {#getColumnIndexes--}
```
public int[] getColumnIndexes()
```


Gets or sets the columns(0-based) to import from data source. null means all columns should be imported.

**Returns:**
int[]
### getConvertGridStyle() {#getConvertGridStyle--}
```
public boolean getConvertGridStyle()
```


Indicates whether apply the style of the grid view to cells.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Gets or sets a value that indicates whether the string value should be converted to numeric or date value.

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


Gets or sets date format string for cells with imported datetime values.

**Returns:**
java.lang.String
### getDefaultValues() {#getDefaultValues--}
```
public Object[] getDefaultValues()
```


Default value for the value in the table is null.

**Returns:**
java.lang.Object[]
### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}
```
public boolean getExportCaptionAsFieldName()
```


Indicates whether exporting caption as field name Only works for DataTable.

**Returns:**
boolean
### getInsertRows() {#getInsertRows--}
```
public boolean getInsertRows()
```


Indicates whether new rows should be added for importing data records.

**Returns:**
boolean
### getNumberFormats() {#getNumberFormats--}
```
public String[] getNumberFormats()
```


Gets or sets the number formats

**Returns:**
java.lang.String[]
### getShiftFirstRowDown() {#getShiftFirstRowDown--}
```
public boolean getShiftFirstRowDown()
```


Indicates whether shifting the first row down when inserting rows.

**Returns:**
boolean
### getTotalColumns() {#getTotalColumns--}
```
public int getTotalColumns()
```


Gets or sets total column count to import from data source. -1 means all rows of given data source.

**Returns:**
int
### getTotalRows() {#getTotalRows--}
```
public int getTotalRows()
```


Gets or sets total row count to import from data source. -1 means all rows of given data source.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFieldNameShown() {#isFieldNameShown--}
```
public boolean isFieldNameShown()
```


Indicates whether field name should be imported.

**Returns:**
boolean
### isFormulas() {#isFormulas--}
```
public boolean[] isFormulas()
```


Indicates whether the data are formulas.

**Returns:**
boolean[]
### isHtmlString() {#isHtmlString--}
```
public boolean isHtmlString()
```


Indicates whether the value contains html tags.

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




### setCheckMergedCells(boolean value) {#setCheckMergedCells-boolean-}
```
public void setCheckMergedCells(boolean value)
```


For the description of this property, please see \#getCheckMergedCells().getCheckMergedCells()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setColumnIndexes(int[] value) {#setColumnIndexes-int---}
```
public void setColumnIndexes(int[] value)
```


For the description of this property, please see \#getColumnIndexes().getColumnIndexes()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int[] |  |

### setConvertGridStyle(boolean value) {#setConvertGridStyle-boolean-}
```
public void setConvertGridStyle(boolean value)
```


For the description of this property, please see \#getConvertGridStyle().getConvertGridStyle()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


For the description of this property, please see \#getConvertNumericData().getConvertNumericData()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


For the description of this property, please see \#getDateFormat().getDateFormat()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDefaultValues(Object[] value) {#setDefaultValues-java.lang.Object---}
```
public void setDefaultValues(Object[] value)
```


For the description of this property, please see \#getDefaultValues().getDefaultValues()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object[] |  |

### setExportCaptionAsFieldName(boolean value) {#setExportCaptionAsFieldName-boolean-}
```
public void setExportCaptionAsFieldName(boolean value)
```


For the description of this property, please see \#getExportCaptionAsFieldName().getExportCaptionAsFieldName()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFieldNameShown(boolean value) {#setFieldNameShown-boolean-}
```
public void setFieldNameShown(boolean value)
```


For the description of this property, please see \#isFieldNameShown().isFieldNameShown()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFormulas(boolean[] value) {#setFormulas-boolean---}
```
public void setFormulas(boolean[] value)
```


For the description of this property, please see \#isFormulas().isFormulas()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean[] |  |

### setHtmlString(boolean value) {#setHtmlString-boolean-}
```
public void setHtmlString(boolean value)
```


For the description of this property, please see \#isHtmlString().isHtmlString()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInsertRows(boolean value) {#setInsertRows-boolean-}
```
public void setInsertRows(boolean value)
```


For the description of this property, please see \#getInsertRows().getInsertRows()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNumberFormats(String[] value) {#setNumberFormats-java.lang.String---}
```
public void setNumberFormats(String[] value)
```


For the description of this property, please see \#getNumberFormats().getNumberFormats()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String[] |  |

### setShiftFirstRowDown(boolean value) {#setShiftFirstRowDown-boolean-}
```
public void setShiftFirstRowDown(boolean value)
```


For the description of this property, please see \#getShiftFirstRowDown().getShiftFirstRowDown()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTotalColumns(int value) {#setTotalColumns-int-}
```
public void setTotalColumns(int value)
```


For the description of this property, please see \#getTotalColumns().getTotalColumns()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTotalRows(int value) {#setTotalRows-int-}
```
public void setTotalRows(int value)
```


For the description of this property, please see \#getTotalRows().getTotalRows()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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

