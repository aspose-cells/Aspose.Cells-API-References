---
title: ListObject
second_title: Aspose.Cells for Java API Reference
description: Represents a table in a worksheet.
type: docs
url: /java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

Represents a table in a worksheet.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         table.getListColumns().get(4).setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         workbook.save("Book1.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [applyStyleToRange()](#applyStyleToRange--) | Apply the table style to the range. |
| [convertToRange()](#convertToRange--) | Convert the table to range. |
| [convertToRange(TableToRangeOptions options)](#convertToRange-com.aspose.cells.TableToRangeOptions-) | Convert the table to range. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter()](#filter--) | Filter the table. |
| [getAlternativeDescription()](#getAlternativeDescription--) | Gets the alternative description. |
| [getAlternativeText()](#getAlternativeText--) | Gets the alternative text. |
| [getAutoFilter()](#getAutoFilter--) | Gets auto filter of this table. |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Gets the comment of the table. |
| [getDataRange()](#getDataRange--) | Gets the data range of the Table. |
| [getDataSourceType()](#getDataSourceType--) | Gets the data source type of the table. |
| [getDisplayName()](#getDisplayName--) | Gets the display name of the table. |
| [getEndColumn()](#getEndColumn--) | Gets the end column of the range. |
| [getEndRow()](#getEndRow--) | Gets the end row of the range. |
| [getListColumns()](#getListColumns--) | Gets the [ListColumn](../../com.aspose.cells/listcolumn) list of this table. |
| [getQueryTable()](#getQueryTable--) | Gets the linked QueryTable. |
| [getShowHeaderRow()](#getShowHeaderRow--) | Gets whether this Table shows header row. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | Indicates whether column stripe formatting is applied to. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | Indicates whether the first column in the table is the style applied to. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | Indicates whether the last column in the table is the style applied to. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | Indicates whether row stripe formatting is applied to. |
| [getShowTotals()](#getShowTotals--) | Gets whether this TAble shows total row. |
| [getStartColumn()](#getStartColumn--) | Gets the start column of the range. |
| [getStartRow()](#getStartRow--) | Gets the start row of the range. |
| [getTableStyleName()](#getTableStyleName--) | Gets the table style name. |
| [getTableStyleType()](#getTableStyleType--) | Gets and the built-in table style. |
| [getXmlMap()](#getXmlMap--) | Gets an [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) used for this list. |
| [hasAutoFilter()](#hasAutoFilter--) | Indicates whether auto filter is applied to this table. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellFormula(int rowOffset, int columnOffset, String formula)](#putCellFormula-int-int-java.lang.String-) | Put the formula to the cell in the table. |
| [putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)](#putCellFormula-int-int-java.lang.String-boolean-) | Put the formula to the cell in the table. |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | Put the value to the cell. |
| [putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)](#putCellValue-int-int-java.lang.Object-boolean-) | Put the value to the cell. |
| [removeAutoFilter()](#removeAutoFilter--) | Removes auto filter which is applied to this table. |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | Resize the range of the list object. |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | Sets the alternative description. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Sets the alternative text. |
| [setComment(String value)](#setComment-java.lang.String-) | Sets the comment of the table. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Sets the display name of the table. |
| [setHasAutoFilter(boolean value)](#setHasAutoFilter-boolean-) | Indicates whether auto filter is applied to this table. |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | Sets whether this Table shows header row. |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | Indicates whether column stripe formatting is applied to. |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | Indicates whether the first column in the table is the style applied to. |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | Indicates whether the last column in the table is the style applied to. |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | Indicates whether row stripe formatting is applied to. |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | Sets whether this TAble shows total row. |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | Sets the table style name. |
| [setTableStyleType(int value)](#setTableStyleType-int-) | Gets and the built-in table style. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Updates all list columns' name to cells in the table. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyleToRange() {#applyStyleToRange--}
```
public void applyStyleToRange()
```


Apply the table style to the range.

### convertToRange() {#convertToRange--}
```
public void convertToRange()
```


Convert the table to range.

### convertToRange(TableToRangeOptions options) {#convertToRange-com.aspose.cells.TableToRangeOptions-}
```
public void convertToRange(TableToRangeOptions options)
```


Convert the table to range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [TableToRangeOptions](../../com.aspose.cells/tabletorangeoptions) | the options when converting table to range. |

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
### filter() {#filter--}
```
public AutoFilter filter()
```


Filter the table.

**Remarks**

NOTE: This member is now obsolete. Instead,please set ListObject.HasAutoFilter property./// This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


Gets the alternative description.

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Gets the alternative text.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Gets auto filter of this table.

**Remarks**

It works only when [hasAutoFilter()](../../com.aspose.cells/listobject\#hasAutoFilter--) is false.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```


Gets the comment of the table.

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


Gets the data range of the Table.

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


Gets the data source type of the table.

See [TableDataSourceType](../../com.aspose.cells/tabledatasourcetype).

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Gets the display name of the table.

**Returns:**
java.lang.String
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Gets the end column of the range.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Gets the end row of the range.

**Returns:**
int
### getListColumns() {#getListColumns--}
```
public ListColumnCollection getListColumns()
```


Gets the [ListColumn](../../com.aspose.cells/listcolumn) list of this table.

**Returns:**
[ListColumnCollection](../../com.aspose.cells/listcolumncollection)
### getQueryTable() {#getQueryTable--}
```
public QueryTable getQueryTable()
```


Gets the linked QueryTable.

**Returns:**
[QueryTable](../../com.aspose.cells/querytable)
### getShowHeaderRow() {#getShowHeaderRow--}
```
public boolean getShowHeaderRow()
```


Gets whether this Table shows header row.

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


Indicates whether column stripe formatting is applied to.

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


Indicates whether the first column in the table is the style applied to.

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


Indicates whether the last column in the table is the style applied to.

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


Indicates whether row stripe formatting is applied to.

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


Gets whether this TAble shows total row.

**Returns:**
boolean
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Gets the start column of the range.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Gets the start row of the range.

**Returns:**
int
### getTableStyleName() {#getTableStyleName--}
```
public String getTableStyleName()
```


Gets the table style name.

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


Gets and the built-in table style.

See [TableStyleType](../../com.aspose.cells/tablestyletype).

**Example**

```
         Workbook workbook = new Workbook("Book1.xlsx");
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setTableStyleType(TableStyleType.TABLE_STYLE_DARK_2);
          workbook.save("TableStyle.xlsx");
```

**Returns:**
int
### getXmlMap() {#getXmlMap--}
```
public XmlMap getXmlMap()
```


Gets an [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) used for this list.

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap)
### hasAutoFilter() {#hasAutoFilter--}
```
public boolean hasAutoFilter()
```


Indicates whether auto filter is applied to this table.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putCellFormula(int rowOffset, int columnOffset, String formula) {#putCellFormula-int-int-java.lang.String-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula)
```


Put the formula to the cell in the table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | The row offset in the table. |
| columnOffset | int | The column offset in the table. |
| formula | java.lang.String | The formula of the cell. |

### putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula) {#putCellFormula-int-int-java.lang.String-boolean-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)
```


Put the formula to the cell in the table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | The row offset in the table. |
| columnOffset | int | The column offset in the table. |
| formula | java.lang.String | The formula of the cell. |
| isTotalsRowFormula | boolean |  |

### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


Put the value to the cell.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | The row offset in the table. |
| columnOffset | int | The column offset in the table. |
| value | java.lang.Object | The cell value. |

### putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel) {#putCellValue-int-int-java.lang.Object-boolean-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)
```


Put the value to the cell.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | The row offset in the table. |
| columnOffset | int | The column offset in the table. |
| value | java.lang.Object | The cell value. |
| isTotalsRowLabel | boolean | Indicates whether it is a label for total row,only works for total row. If False and this row is total row, a new row will be inserted. |

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Removes auto filter which is applied to this table.

### resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#resize-int-int-int-int-boolean-}
```
public void resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Resize the range of the list object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row index of the new range. |
| startColumn | int | The start column index of the new range. |
| endRow | int | The end row index of the new range. |
| endColumn | int | The end column index of the new range. |
| hasHeaders | boolean | Whether this table has headers. |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


Sets the alternative description.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Sets the alternative text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Sets the comment of the table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Sets the display name of the table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setHasAutoFilter(boolean value) {#setHasAutoFilter-boolean-}
```
public void setHasAutoFilter(boolean value)
```


Indicates whether auto filter is applied to this table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


Sets whether this Table shows header row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


Indicates whether column stripe formatting is applied to.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


Indicates whether the first column in the table is the style applied to.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


Indicates whether the last column in the table is the style applied to.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


Indicates whether row stripe formatting is applied to.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


Sets whether this TAble shows total row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


Sets the table style name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


Gets and the built-in table style.

See [TableStyleType](../../com.aspose.cells/tablestyletype).

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
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Updates all list columns' name to cells in the table.

**Remarks**

The value of the cells in the header row of the table must be same as the name of the ListColumn; Cell.PutValue do not auto modify the name of the ListColumn for performance.

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

