---
title: "AutoFilter"
second_title: "Aspose.Cells for Java API 参考"
description: "表示对指定工作表的自动筛选。"
type: docs
url: /zh/java/com.aspose.cells/autofilter/
---

**Inheritance:**
java.lang.Object
```
public class AutoFilter
```

表示对指定工作表的自动筛选。

**Example**

```
         //Creating a file stream containing the Excel file to be opened
         //Instantiating a Workbook object
         Workbook workbook = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating AutoFilter by giving the cells range of the heading row
         worksheet.getAutoFilter().setRange("A1:B1");
         //Filtering columns with specified values
         worksheet.getAutoFilter().filter(1, "Bananas");
         //Saving the modified Excel file.
         workbook.save("output.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#addDateFilter-int-int-int-int-int-int-int-int-) | 添加日期过滤器。 |
| [addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)](#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-) | 添加填充颜色过滤器。 |
| [addFilter(int fieldIndex, String criteria)](#addFilter-int-java.lang.String-) | 为过滤列添加过滤器。 |
| [addFontColorFilter(int fieldIndex, CellsColor color)](#addFontColorFilter-int-com.aspose.cells.CellsColor-) | 添加字体颜色过滤器。 |
| [addIconFilter(int fieldIndex, int iconSetType, int iconId)](#addIconFilter-int-int-int-) | 添加图标过滤器。 |
| [custom(int fieldIndex, int operatorType1, Object criteria1)](#custom-int-int-java.lang.Object-) | 使用自定义条件过滤列表。 |
| [custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-) | 使用自定义标准过滤列表。 |
| [dynamicFilter(int fieldIndex, int dynamicFilterType)](#dynamicFilter-int-int-) | 添加动态过滤器。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int fieldIndex, String criteria)](#filter-int-java.lang.String-) | 使用指定的条件过滤列表。 |
| [filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)](#filterTop10-int-boolean-boolean-int-) | 筛选列表中的前10项 |
| [getCellArea()](#getCellArea--) | 获取此自动筛选适用的 [CellArea](../../com.aspose.cells/cellarea)。 |
| [getCellArea(boolean refreshAppliedRange)](#getCellArea-boolean-) | 获取指定自动筛选适用的 [CellArea](../../com.aspose.cells/cellarea)。 |
| [getClass()](#getClass--) |  |
| [getFilterColumns()](#getFilterColumns--) | 获取筛选列的集合。 |
| [getRange()](#getRange--) | 表示指定自动筛选适用的范围。 |
| [getShowFilterButton()](#getShowFilterButton--) | 指示此列的自动筛选按钮是否可见。 |
| [getSorter()](#getSorter--) | 获取数据排序器。 |
| [hashCode()](#hashCode--) |  |
| [matchBlanks(int fieldIndex)](#matchBlanks-int-) | 匹配列表中所有空白单元格。 |
| [matchNonBlanks(int fieldIndex)](#matchNonBlanks-int-) | 匹配列表中所有非空白单元格。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | 刷新自动筛选以隐藏或显示行。 |
| [refresh(boolean hideRows)](#refresh-boolean-) | 获取所有隐藏行的索引。 |
| [removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#removeDateFilter-int-int-int-int-int-int-int-int-) | 移除日期筛选。 |
| [removeFilter(int fieldIndex)](#removeFilter-int-) | 移除特定筛选。 |
| [removeFilter(int fieldIndex, String criteria)](#removeFilter-int-java.lang.String-) | 移除筛选列的筛选。 |
| [setRange(int row, int startColumn, int endColumn)](#setRange-int-int-int-) | 设置指定自动筛选适用的范围。 |
| [setRange(String value)](#setRange-java.lang.String-) | 表示指定自动筛选适用的范围。 |
| [setShowFilterButton(boolean value)](#setShowFilterButton-boolean-) | 指示此列的自动筛选按钮是否可见。 |
| [showAll()](#showAll--) | 显示所有行。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#addDateFilter-int-int-int-int-int-int-int-int-}
```
public void addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


添加日期过滤器。

**Remarks**

如果 DateTimeGroupingType 为 Year，则仅参数 year 生效。如果 DateTiemGroupingType 为 Month，则仅参数 year 和 month 生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). 分组类型 |
| 年 | int | 年份。 |
| 月 | int | 月份。 |
| 日 | int | 日期。 |
| 小时 | int | 小时。 |
| 分钟 | int | 分钟。 |
| 秒 | int | 秒。 |

### addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor) {#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-}
```
public void addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)
```


添加填充颜色过滤器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). 背景图案类型。 |
| foregroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | 前景色。 |
| backgroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | 背景色。 |

### addFilter(int fieldIndex, String criteria) {#addFilter-int-java.lang.String-}
```
public void addFilter(int fieldIndex, String criteria)
```


为过滤列添加过滤器。

**Remarks**

MS Excel 2007 支持在筛选列中进行多选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| 条件 | java.lang.String | 指定的条件（字符串；例如，\"101\"）。它只能为 null 或该列中单元格的某个值。 |

### addFontColorFilter(int fieldIndex, CellsColor color) {#addFontColorFilter-int-com.aspose.cells.CellsColor-}
```
public void addFontColorFilter(int fieldIndex, CellsColor color)
```


添加字体颜色过滤器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| color | [CellsColor](../../com.aspose.cells/cellscolor) | [CellsColor](../../com.aspose.cells/cellscolor) 对象。 |

### addIconFilter(int fieldIndex, int iconSetType, int iconId) {#addIconFilter-int-int-int-}
```
public void addIconFilter(int fieldIndex, int iconSetType, int iconId)
```


添加图标过滤器。

**Remarks**

仅支持添加图标筛选器。不支持检查在图标筛选器情况下哪一行可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| iconSetType | int | [IconSetType](../../com.aspose.cells/iconsettype)。图标集合类型。 |
| iconId | int | 图标 ID。 |

### custom(int fieldIndex, int operatorType1, Object criteria1) {#custom-int-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1)
```


使用自定义条件过滤列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype)。筛选运算符类型 |
| criteria1 | java.lang.Object | 自定义条件 |

### custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


使用自定义标准过滤列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype)。筛选运算符类型 |
| criteria1 | java.lang.Object | 自定义条件 |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype)。筛选运算符类型 |
| criteria2 | java.lang.Object | 自定义条件 |

### dynamicFilter(int fieldIndex, int dynamicFilterType) {#dynamicFilter-int-int-}
```
public void dynamicFilter(int fieldIndex, int dynamicFilterType)
```


添加动态过滤器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| dynamicFilterType | int | [DynamicFilterType](../../com.aspose.cells/dynamicfiltertype)。动态筛选类型。 |

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
### filter(int fieldIndex, String criteria) {#filter-int-java.lang.String-}
```
public void filter(int fieldIndex, String criteria)
```


使用指定的条件过滤列表。

**Remarks**

Aspose.Cells 将删除此字段上所有其他筛选设置，类似于 MS Excel 97-2003。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| 条件 | java.lang.String | 指定的条件（字符串；例如，\"101\"）。 |

### filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount) {#filterTop10-int-boolean-boolean-int-}
```
public void filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)
```


筛选列表中的前10项

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| isTop | boolean | 指示过滤是来自顶部还是底部 |
| isPercent | boolean | 指示项目是百分比还是计数 |
| itemCount | int | 项目计数 |

### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


获取此自动筛选适用的 [CellArea](../../com.aspose.cells/cellarea)。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getCellArea(boolean refreshAppliedRange) {#getCellArea-boolean-}
```
public CellArea getCellArea(boolean refreshAppliedRange)
```


获取指定自动筛选适用的 [CellArea](../../com.aspose.cells/cellarea)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| refreshAppliedRange | boolean | 是否刷新已应用的范围。对于自动筛选的已应用范围，当单元格数据更改时，最后一行可能会变化。如果此标志为 true，则范围的最后一行将根据当前单元格数据重新计算。 |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilterColumns() {#getFilterColumns--}
```
public FilterColumnCollection getFilterColumns()
```


获取筛选列的集合。

**Returns:**
[FilterColumnCollection](../../com.aspose.cells/filtercolumncollection)
### getRange() {#getRange--}
```
public String getRange()
```


表示指定自动筛选适用的范围。

**Returns:**
java.lang.String
### getShowFilterButton() {#getShowFilterButton--}
```
public boolean getShowFilterButton()
```


指示此列的自动筛选按钮是否可见。

**Returns:**
boolean
### getSorter() {#getSorter--}
```
public DataSorter getSorter()
```


获取数据排序器。

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### matchBlanks(int fieldIndex) {#matchBlanks-int-}
```
public void matchBlanks(int fieldIndex)
```


匹配列表中所有空白单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |

### matchNonBlanks(int fieldIndex) {#matchNonBlanks-int-}
```
public void matchNonBlanks(int fieldIndex)
```


匹配列表中所有非空白单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int[] refresh()
```


刷新自动筛选以隐藏或显示行。

**Returns:**
int[] - 返回所有隐藏行的索引。
### refresh(boolean hideRows) {#refresh-boolean-}
```
public int[] refresh(boolean hideRows)
```


获取所有隐藏行的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| hideRows | boolean | 如果为 true，隐藏已筛选的行。 |

**Returns:**
int[] - 返回所有隐藏行的索引。
### removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#removeDateFilter-int-int-int-int-int-int-int-int-}
```
public void removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


移除日期筛选。

**Remarks**

如果 DateTimeGroupingType 为 Year，则仅参数 year 生效。如果 DateTiemGroupingType 为 Month，则仅参数 year 和 month 生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). 分组类型 |
| 年 | int | 年份。 |
| 月 | int | 月份。 |
| 日 | int | 日期。 |
| 小时 | int | 小时。 |
| 分钟 | int | 分钟。 |
| 秒 | int | 秒。 |

### removeFilter(int fieldIndex) {#removeFilter-int-}
```
public void removeFilter(int fieldIndex)
```


移除特定筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 特定过滤器索引 |

### removeFilter(int fieldIndex, String criteria) {#removeFilter-int-java.lang.String-}
```
public void removeFilter(int fieldIndex, String criteria)
```


移除筛选列的筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int | 要基于其进行筛选的字段的整数偏移量（相对于列表左侧；最左侧字段为字段 0）。 |
| 条件 | java.lang.String | 指定的条件（字符串；例如，\"101\"）。它只能为 null 或该列中单元格的某个值。 |

### setRange(int row, int startColumn, int endColumn) {#setRange-int-int-int-}
```
public void setRange(int row, int startColumn, int endColumn)
```


设置指定自动筛选适用的范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| startColumn | int | 起始列索引。 |
| endColumn | int | 结束列索引。 |

### setRange(String value) {#setRange-java.lang.String-}
```
public void setRange(String value)
```


表示指定自动筛选适用的范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setShowFilterButton(boolean value) {#setShowFilterButton-boolean-}
```
public void setShowFilterButton(boolean value)
```


指示此列的自动筛选按钮是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### showAll() {#showAll--}
```
public void showAll()
```


显示所有行。

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

