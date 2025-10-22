##ImportTableOptions
Represents the options of importing data into cells.
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
| [getColumnIndexes()](#getColumnIndexes--) | Gets the columns(0-based) to import from data source. null means all columns should be imported. |
| [getConvertGridStyle()](#getConvertGridStyle--) | Indicates whether apply the style of the grid view to cells. |
| [getConvertNumericData()](#getConvertNumericData--) | Gets a value that indicates whether the string value should be converted to numeric or date value. |
| [getDateFormat()](#getDateFormat--) | Gets date format string for cells with imported datetime values. |
| [getDefaultValues()](#getDefaultValues--) | Default value for the value in the table is null. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--) | Indicates whether exporting caption as field name |
| [getInsertRows()](#getInsertRows--) | Indicates whether new rows should be added for importing data records. |
| [getNumberFormats()](#getNumberFormats--) | Gets the number formats |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--) | Indicates whether shifting the first row down when inserting rows. |
| [getTotalColumns()](#getTotalColumns--) | Gets total column count to import from data source. -1 means all rows of given data source. |
| [getTotalRows()](#getTotalRows--) | Gets total row count to import from data source. -1 means all rows of given data source. |
| [hashCode()](#hashCode--) |  |
| [isFieldNameShown()](#isFieldNameShown--) | Indicates whether field name should be imported. |
| [isFormulas()](#isFormulas--) | Indicates whether the data are formulas. |
| [isHtmlString()](#isHtmlString--) | Indicates whether the value contains html tags. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMergedCells(boolean value)](#setCheckMergedCells-boolean-) | Indicates whether checking merged cells. |
| [setColumnIndexes(int[] value)](#setColumnIndexes-int---) | Sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [setConvertGridStyle(boolean value)](#setConvertGridStyle-boolean-) | Indicates whether apply the style of the grid view to cells. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Sets a value that indicates whether the string value should be converted to numeric or date value. |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | Sets date format string for cells with imported datetime values. |
| [setDefaultValues(Object[] value)](#setDefaultValues-java.lang.Object---) | Default value for the value in the table is null. |
| [setExportCaptionAsFieldName(boolean value)](#setExportCaptionAsFieldName-boolean-) | Indicates whether exporting caption as field name |
| [setFieldNameShown(boolean value)](#setFieldNameShown-boolean-) | Indicates whether field name should be imported. |
| [setFormulas(boolean[] value)](#setFormulas-boolean---) | Indicates whether the data are formulas. |
| [setHtmlString(boolean value)](#setHtmlString-boolean-) | Indicates whether the value contains html tags. |
| [setInsertRows(boolean value)](#setInsertRows-boolean-) | Indicates whether new rows should be added for importing data records. |
| [setNumberFormats(String[] value)](#setNumberFormats-java.lang.String---) | Sets the number formats |
| [setShiftFirstRowDown(boolean value)](#setShiftFirstRowDown-boolean-) | Indicates whether shifting the first row down when inserting rows. |
| [setTotalColumns(int value)](#setTotalColumns-int-) | Sets total column count to import from data source. -1 means all rows of given data source. |
| [setTotalRows(int value)](#setTotalRows-int-) | Sets total row count to import from data source. -1 means all rows of given data source. |
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
Gets the columns(0-based) to import from data source. null means all columns should be imported.
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
Gets a value that indicates whether the string value should be converted to numeric or date value.
**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```
Gets date format string for cells with imported datetime values.
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
Indicates whether exporting caption as field name
**Remarks**
Only works for DataTable.
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
Gets the number formats
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
Gets total column count to import from data source. -1 means all rows of given data source.
**Returns:**
int
### getTotalRows() {#getTotalRows--}
```
public int getTotalRows()
```
Gets total row count to import from data source. -1 means all rows of given data source.
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
Indicates whether checking merged cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setColumnIndexes(int[] value) {#setColumnIndexes-int---}
```
public void setColumnIndexes(int[] value)
```
Sets the columns(0-based) to import from data source. null means all columns should be imported.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int[] |  |
### setConvertGridStyle(boolean value) {#setConvertGridStyle-boolean-}
```
public void setConvertGridStyle(boolean value)
```
Indicates whether apply the style of the grid view to cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```
Sets a value that indicates whether the string value should be converted to numeric or date value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```
Sets date format string for cells with imported datetime values.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setDefaultValues(Object[] value) {#setDefaultValues-java.lang.Object---}
```
public void setDefaultValues(Object[] value)
```
Default value for the value in the table is null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object[] |  |
### setExportCaptionAsFieldName(boolean value) {#setExportCaptionAsFieldName-boolean-}
```
public void setExportCaptionAsFieldName(boolean value)
```
Indicates whether exporting caption as field name
**Remarks**
Only works for DataTable.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFieldNameShown(boolean value) {#setFieldNameShown-boolean-}
```
public void setFieldNameShown(boolean value)
```
Indicates whether field name should be imported.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFormulas(boolean[] value) {#setFormulas-boolean---}
```
public void setFormulas(boolean[] value)
```
Indicates whether the data are formulas.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean[] |  |
### setHtmlString(boolean value) {#setHtmlString-boolean-}
```
public void setHtmlString(boolean value)
```
Indicates whether the value contains html tags.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setInsertRows(boolean value) {#setInsertRows-boolean-}
```
public void setInsertRows(boolean value)
```
Indicates whether new rows should be added for importing data records.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setNumberFormats(String[] value) {#setNumberFormats-java.lang.String---}
```
public void setNumberFormats(String[] value)
```
Sets the number formats
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String[] |  |
### setShiftFirstRowDown(boolean value) {#setShiftFirstRowDown-boolean-}
```
public void setShiftFirstRowDown(boolean value)
```
Indicates whether shifting the first row down when inserting rows.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setTotalColumns(int value) {#setTotalColumns-int-}
```
public void setTotalColumns(int value)
```
Sets total column count to import from data source. -1 means all rows of given data source.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTotalRows(int value) {#setTotalRows-int-}
```
public void setTotalRows(int value)
```
Sets total row count to import from data source. -1 means all rows of given data source.
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
