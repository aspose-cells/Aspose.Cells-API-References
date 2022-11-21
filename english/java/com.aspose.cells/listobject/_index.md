---
title: ListObject
second_title: Aspose.Cells for Java API Reference
description: Represents a list object on a worksheet.
type: docs
weight: 306
url: /java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

Represents a list object on a worksheet. The ListObject object is a member of the ListObjects collection. The ListObjects collection contains all the list objects on a worksheet.

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
| [getAlternativeDescription()](#getAlternativeDescription--) | the alternative description. |
| [getAlternativeText()](#getAlternativeText--) | the alternative text. |
| [getAutoFilter()](#getAutoFilter--) | Gets auto filter. |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | the comment of the table. |
| [getDataRange()](#getDataRange--) | Gets the data range of the ListObject. |
| [getDataSourceType()](#getDataSourceType--) | Gets the data source type of the table. |
| [getDisplayName()](#getDisplayName--) | the display name. |
| [getEndColumn()](#getEndColumn--) | Gets the end column of the range. |
| [getEndRow()](#getEndRow--) | Gets the end row of the range. |
| [getListColumns()](#getListColumns--) | Gets ListColumns of the ListObject. |
| [getQueryTable()](#getQueryTable--) | Gets the linked QueryTable. |
| [getShowHeaderRow()](#getShowHeaderRow--) | whether this ListObject show header row. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | Indicates whether column stripe formatting is applied. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | Indicates whether the first column in the table should have the style applied. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | Indicates whether the last column in the table should have the style applied. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | Indicates whether row stripe formatting is applied. |
| [getShowTotals()](#getShowTotals--) | whether this ListObject show total row. |
| [getStartColumn()](#getStartColumn--) | Gets the start column of the range. |
| [getStartRow()](#getStartRow--) | Gets the start row of the range. |
| [getTableStyleName()](#getTableStyleName--) | the table style name. |
| [getTableStyleType()](#getTableStyleType--) | Gets and the built-in table style. |
| [getXmlMap()](#getXmlMap--) | Gets an [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) used for this list. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | Put the value to the cell. |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | Resize the range of the list object. |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | For the description of this property, please see [getAlternativeDescription()](../../com.aspose.cells/listobject\#getAlternativeDescription--) |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | For the description of this property, please see [getAlternativeText()](../../com.aspose.cells/listobject\#getAlternativeText--) |
| [setComment(String value)](#setComment-java.lang.String-) | For the description of this property, please see [getComment()](../../com.aspose.cells/listobject\#getComment--) |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | For the description of this property, please see [getDisplayName()](../../com.aspose.cells/listobject\#getDisplayName--) |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | For the description of this property, please see [getShowHeaderRow()](../../com.aspose.cells/listobject\#getShowHeaderRow--) |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | For the description of this property, please see [getShowTableStyleColumnStripes()](../../com.aspose.cells/listobject\#getShowTableStyleColumnStripes--) |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | For the description of this property, please see [getShowTableStyleFirstColumn()](../../com.aspose.cells/listobject\#getShowTableStyleFirstColumn--) |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | For the description of this property, please see [getShowTableStyleLastColumn()](../../com.aspose.cells/listobject\#getShowTableStyleLastColumn--) |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | For the description of this property, please see [getShowTableStyleRowStripes()](../../com.aspose.cells/listobject\#getShowTableStyleRowStripes--) |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | For the description of this property, please see [getShowTotals()](../../com.aspose.cells/listobject\#getShowTotals--) |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | For the description of this property, please see [getTableStyleName()](../../com.aspose.cells/listobject\#getTableStyleName--) |
| [setTableStyleType(int value)](#setTableStyleType-int-) | For the description of this property, please see [getTableStyleType()](../../com.aspose.cells/listobject\#getTableStyleType--) |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Updates all list columns' name from the worksheet. |
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

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


the alternative description.

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


the alternative text.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Gets auto filter.

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


the comment of the table.

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


Gets the data range of the ListObject.

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


Gets the data source type of the table.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


the display name.

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


Gets ListColumns of the ListObject.

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


whether this ListObject show header row.

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


Indicates whether column stripe formatting is applied.

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


Indicates whether the first column in the table should have the style applied.

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


Indicates whether the last column in the table should have the style applied.

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


Indicates whether row stripe formatting is applied.

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


whether this ListObject show total row.

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


the table style name.

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


Gets and the built-in table style.

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




### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


Put the value to the cell.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | The row offset. |
| columnOffset | int | The column offset. |
| value | java.lang.Object | The cell value. |

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
| hasHeaders | boolean | Whether the ListObject has headers. |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


For the description of this property, please see [getAlternativeDescription()](../../com.aspose.cells/listobject\#getAlternativeDescription--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


For the description of this property, please see [getAlternativeText()](../../com.aspose.cells/listobject\#getAlternativeText--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


For the description of this property, please see [getComment()](../../com.aspose.cells/listobject\#getComment--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


For the description of this property, please see [getDisplayName()](../../com.aspose.cells/listobject\#getDisplayName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


For the description of this property, please see [getShowHeaderRow()](../../com.aspose.cells/listobject\#getShowHeaderRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


For the description of this property, please see [getShowTableStyleColumnStripes()](../../com.aspose.cells/listobject\#getShowTableStyleColumnStripes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


For the description of this property, please see [getShowTableStyleFirstColumn()](../../com.aspose.cells/listobject\#getShowTableStyleFirstColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


For the description of this property, please see [getShowTableStyleLastColumn()](../../com.aspose.cells/listobject\#getShowTableStyleLastColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


For the description of this property, please see [getShowTableStyleRowStripes()](../../com.aspose.cells/listobject\#getShowTableStyleRowStripes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


For the description of this property, please see [getShowTotals()](../../com.aspose.cells/listobject\#getShowTotals--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


For the description of this property, please see [getTableStyleName()](../../com.aspose.cells/listobject\#getTableStyleName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


For the description of this property, please see [getTableStyleType()](../../com.aspose.cells/listobject\#getTableStyleType--)

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


Updates all list columns' name from the worksheet. The value of the cells in the header row of the table must be same as the name of the ListColumn; Cell.PutValue do not auto modify the name of the ListColumn for performance.

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

