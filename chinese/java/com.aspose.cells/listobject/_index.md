---
title: "ListObject"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作表中的表格。"
type: docs
url: /zh/java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

表示工作表中的表格。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [applyStyleToRange()](#applyStyleToRange--) | 将表格样式应用于范围。 |
| [convertToRange()](#convertToRange--) | 将表格转换为范围。 |
| [convertToRange(TableToRangeOptions options)](#convertToRange-com.aspose.cells.TableToRangeOptions-) | 将表格转换为范围。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter()](#filter--) | 筛选表格。 |
| [getAlternativeDescription()](#getAlternativeDescription--) | 获取替代描述。 |
| [getAlternativeText()](#getAlternativeText--) | 获取替代文本。 |
| [getAutoFilter()](#getAutoFilter--) | 获取此表格的自动筛选。 |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | 获取表格的批注。 |
| [getDataRange()](#getDataRange--) | 获取表格的数据范围。 |
| [getDataSourceType()](#getDataSourceType--) | 获取表格的数据源类型。 |
| [getDisplayName()](#getDisplayName--) | 获取表格的显示名称。 |
| [getEndColumn()](#getEndColumn--) | 获取范围的结束列。 |
| [getEndRow()](#getEndRow--) | 获取范围的结束行。 |
| [getListColumns()](#getListColumns--) | 获取此表格的 [ListColumn](../../com.aspose.cells/listcolumn) 列表。 |
| [getQueryTable()](#getQueryTable--) | 获取链接的 QueryTable。 |
| [getShowHeaderRow()](#getShowHeaderRow--) | 获取此表格是否显示标题行。 |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | 指示是否已对列条纹格式进行应用。 |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | 指示表格中的第一列是否已应用样式。 |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | 指示表格中的最后一列是否已应用样式。 |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | 指示是否已对行条纹格式进行应用。 |
| [getShowTotals()](#getShowTotals--) | 获取此 TAble 是否显示总计行。 |
| [getStartColumn()](#getStartColumn--) | 获取范围的起始列。 |
| [getStartRow()](#getStartRow--) | 获取范围的起始行。 |
| [getTableStyleName()](#getTableStyleName--) | 获取表格样式名称。 |
| [getTableStyleType()](#getTableStyleType--) | 获取内置表格样式。 |
| [getXmlMap()](#getXmlMap--) | 获取用于此列表的 [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--)。 |
| [hasAutoFilter()](#hasAutoFilter--) | 指示是否已对该表应用自动筛选。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellFormula(int rowOffset, int columnOffset, String formula)](#putCellFormula-int-int-java.lang.String-) | 将公式放入表格中的单元格。 |
| [putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)](#putCellFormula-int-int-java.lang.String-boolean-) | 将公式放入表格中的单元格。 |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | 将值放入单元格。 |
| [putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)](#putCellValue-int-int-java.lang.Object-boolean-) | 将值放入单元格。 |
| [removeAutoFilter()](#removeAutoFilter--) | 移除已应用于此表的自动筛选。 |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | 调整列表对象的范围大小。 |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | 设置替代描述。 |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | 设置替代文本。 |
| [setComment(String value)](#setComment-java.lang.String-) | 设置表格的注释。 |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | 设置表格的显示名称。 |
| [setHasAutoFilter(boolean value)](#setHasAutoFilter-boolean-) | 指示是否已对该表应用自动筛选。 |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | 设置此 Table 是否显示标题行。 |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | 指示是否已对列条纹格式进行应用。 |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | 指示表格中的第一列是否已应用样式。 |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | 指示表格中的最后一列是否已应用样式。 |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | 指示是否已对行条纹格式进行应用。 |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | 设置此 TAble 是否显示总计行。 |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | 设置表格样式名称。 |
| [setTableStyleType(int value)](#setTableStyleType-int-) | 获取内置表格样式。 |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | 将所有列表列的名称更新到表格中的单元格。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyleToRange() {#applyStyleToRange--}
```
public void applyStyleToRange()
```


将表格样式应用于范围。

### convertToRange() {#convertToRange--}
```
public void convertToRange()
```


将表格转换为范围。

### convertToRange(TableToRangeOptions options) {#convertToRange-com.aspose.cells.TableToRangeOptions-}
```
public void convertToRange(TableToRangeOptions options)
```


将表格转换为范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [TableToRangeOptions](../../com.aspose.cells/tabletorangeoptions) | 将表格转换为范围时的选项。 |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### filter() {#filter--}
```
public AutoFilter filter()
```


筛选表格。

**Remarks**

注意：此成员现已过时。请改为设置 ListObject.HasAutoFilter 属性。/// 此属性将在自2025年10月起的12个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


获取替代描述。

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


获取替代文本。

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


获取此表格的自动筛选。

**Remarks**

仅在 [hasAutoFilter()](../../com.aspose.cells/listobject\#hasAutoFilter--) 为 false 时才有效。

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


获取表格的批注。

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


获取表格的数据范围。

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


获取表格的数据源类型。

参见 [TableDataSourceType](../../com.aspose.cells/tabledatasourcetype)。

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


获取表格的显示名称。

**Returns:**
java.lang.String
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


获取范围的结束列。

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


获取范围的结束行。

**Returns:**
int
### getListColumns() {#getListColumns--}
```
public ListColumnCollection getListColumns()
```


获取此表格的 [ListColumn](../../com.aspose.cells/listcolumn) 列表。

**Returns:**
[ListColumnCollection](../../com.aspose.cells/listcolumncollection)
### getQueryTable() {#getQueryTable--}
```
public QueryTable getQueryTable()
```


获取链接的 QueryTable。

**Returns:**
[QueryTable](../../com.aspose.cells/querytable)
### getShowHeaderRow() {#getShowHeaderRow--}
```
public boolean getShowHeaderRow()
```


获取此表格是否显示标题行。

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


指示是否已对列条纹格式进行应用。

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


指示表格中的第一列是否已应用样式。

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


指示表格中的最后一列是否已应用样式。

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


指示是否已对行条纹格式进行应用。

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


获取此 TAble 是否显示总计行。

**Returns:**
boolean
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


获取范围的起始列。

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


获取范围的起始行。

**Returns:**
int
### getTableStyleName() {#getTableStyleName--}
```
public String getTableStyleName()
```


获取表格样式名称。

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


获取内置表格样式。

参见 [TableStyleType](../../com.aspose.cells/tablestyletype)。

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


获取用于此列表的 [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--)。

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap)
### hasAutoFilter() {#hasAutoFilter--}
```
public boolean hasAutoFilter()
```


指示是否已对该表应用自动筛选。

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


将公式放入表格中的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | int | 表格中的行偏移量。 |
| columnOffset | int | 表格中的列偏移量。 |
| formula | java.lang.String | 单元格的公式。 |

### putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula) {#putCellFormula-int-int-java.lang.String-boolean-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)
```


将公式放入表格中的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | int | 表格中的行偏移量。 |
| columnOffset | int | 表格中的列偏移量。 |
| formula | java.lang.String | 单元格的公式。 |
| isTotalsRowFormula | boolean |  |

### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


将值放入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | int | 表格中的行偏移量。 |
| columnOffset | int | 表格中的列偏移量。 |
| 值 | java.lang.Object | 单元格的值。 |

### putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel) {#putCellValue-int-int-java.lang.Object-boolean-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)
```


将值放入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | int | 表格中的行偏移量。 |
| columnOffset | int | 表格中的列偏移量。 |
| 值 | java.lang.Object | 单元格的值。 |
| isTotalsRowLabel | boolean | 指示它是否为总计行的标签，仅在总计行时有效。如果为 False 且此行为总计行，则会插入新行。 |

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


移除已应用于此表的自动筛选。

### resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#resize-int-int-int-int-boolean-}
```
public void resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


调整列表对象的范围大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 新范围的起始行索引。 |
| startColumn | int | 新范围的起始列索引。 |
| endRow | int | 新范围的结束行索引。 |
| endColumn | int | 新范围的结束列索引。 |
| hasHeaders | boolean | 此表是否具有标题行。 |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


设置替代描述。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


设置替代文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


设置表格的注释。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


设置表格的显示名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setHasAutoFilter(boolean value) {#setHasAutoFilter-boolean-}
```
public void setHasAutoFilter(boolean value)
```


指示是否已对该表应用自动筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


设置此 Table 是否显示标题行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


指示是否已对列条纹格式进行应用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


指示表格中的第一列是否已应用样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


指示表格中的最后一列是否已应用样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


指示是否已对行条纹格式进行应用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


设置此 TAble 是否显示总计行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


设置表格样式名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


获取内置表格样式。

参见 [TableStyleType](../../com.aspose.cells/tablestyletype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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


将所有列表列的名称更新到表格中的单元格。

**Remarks**

表格标题行中单元格的值必须与 ListColumn 的名称相同；为提升性能，Cell.PutValue 不会自动修改 ListColumn 的名称。

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

