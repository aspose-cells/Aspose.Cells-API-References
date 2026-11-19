---
title: "PivotField"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据透视表报告中的字段。"
type: docs
url: /zh/java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

表示数据透视表报告中的字段。

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
          //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
          pivot.calculateData(new PivotTableCalculateOption());
 
         //do your business
 
         book.save("out.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | 向透视字段添加计算公式项。 |
| [clearFilter()](#clearFilter--) | 清除此透视字段的筛选设置。 |
| [dispose()](#dispose--) | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterByDate(int type, DateTime dateTime1, DateTime dateTime2)](#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | 按行或列透视字段的日期值进行筛选。 |
| [filterByLabel(int type, String label1, String label2)](#filterByLabel-int-java.lang.String-java.lang.String-) | 按行或列透视字段的标题进行筛选。 |
| [filterByValue(int valueFieldIndex, int type, double value1, double value2)](#filterByValue-int-int-double-double-) | 按数据透视字段的值进行筛选。 |
| [filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)](#filterTop10-int-int-boolean-int-) | 按数据透视字段的值进行筛选。 |
| [getAllowDraggingToColumn()](#getAllowDraggingToColumn--) | 指示指定字段是否可以拖动到列区域。 |
| [getAllowDraggingToData()](#getAllowDraggingToData--) | 指示指定字段是否可以拖动到值区域。 |
| [getAllowDraggingToPage()](#getAllowDraggingToPage--) | 指示指定字段是否可以拖动到页面区域。 |
| [getAllowDraggingToRow()](#getAllowDraggingToRow--) | 指示指定字段是否可以拖动到行区域。 |
| [getAllowRemovingFromView()](#getAllowRemovingFromView--) | 指示是否可以从数据透视表视图中移除此透视字段。 |
| [getAutoShowCount()](#getAutoShowCount--) | 表示在指定的 PivotTable 字段中自动显示的前或后项目的数量。 |
| [getAutoShowField()](#getAutoShowField--) | 表示自动显示字段索引。-1 表示 PivotField 本身。 |
| [getAutoSortField()](#getAutoSortField--) | 表示自动排序字段的索引 |
| [getBaseIndex()](#getBaseIndex--) | 表示源透视字段中的索引。 |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | 获取指定计算字段的公式字符串。 |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | 获取此透视字段当前显示的页面项（仅限页面字段）。 |
| [getCurrentPageItemText()](#getCurrentPageItemText--) | 获取此透视字段当前页面项的显示文本（仅限页面字段）。 |
| [getDisplayName()](#getDisplayName--) | 表示数据透视表视图中透视字段的显示名称。 |
| [getDragToColumn()](#getDragToColumn--) | 指示指定字段是否可以拖动到列区域。 |
| [getDragToData()](#getDragToData--) | 指示指定字段是否可以拖动到值区域。 |
| [getDragToHide()](#getDragToHide--) | 指示是否可以从数据透视表视图中移除此透视字段。 |
| [getDragToPage()](#getDragToPage--) | 指示指定字段是否可以拖动到页面区域。 |
| [getDragToRow()](#getDragToRow--) | 指示指定字段是否可以拖动到行区域。 |
| [getFilters()](#getFilters--) | 获取此透视字段应用的所有透视筛选器。 |
| [getFormula()](#getFormula--) | 获取计算字段的公式。 |
| [getFunction()](#getFunction--) | 表示用于汇总此数据透视表数据字段的函数。 |
| [getGroupSettings()](#getGroupSettings--) | 获取透视字段的分组设置。 |
| [getInsertBlankRow()](#getInsertBlankRow--) | 指示是否在每个项目后插入空行。 |
| [getItemCount()](#getItemCount--) | 获取此透视字段中基础项目的计数。 |
| [getItems()](#getItems--) | 获取此字段中透视项目的所有标签。 |
| [getMaxValue()](#getMaxValue--) | 获取此字段的最大值。 |
| [getMinValue()](#getMinValue--) | 获取此字段的最大值。 |
| [getName()](#getName--) | 表示 PivotField 的名称。 |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | 指示将应用于此透视字段的排序操作是自动排序还是简单数据排序。 |
| [getNumber()](#getNumber--) | 表示数字和日期的内置显示格式。 |
| [getNumberFormat()](#getNumberFormat--) | 表示数字和日期的自定义显示格式。 |
| [getOriginalItems()](#getOriginalItems--) | 获取原始基础项目； |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | 获取按类型划分的透视字段的透视过滤器 |
| [getPivotFilters()](#getPivotFilters--) | 获取透视字段的透视过滤器 |
| [getPivotItems()](#getPivotItems--) | 获取透视字段的透视项目 |
| [getPosition()](#getPosition--) | 表示区域中 [PivotField](../../com.aspose.cells/pivotfield) 的索引。 |
| [getRegionType()](#getRegionType--) | 指定此字段显示的透视表区域。 |
| [getShowAllItems()](#getShowAllItems--) | 指示是否在 PivotTable 视图中显示所有项目，即使它们不包含汇总数据。 |
| [getShowCompact()](#getShowCompact--) | 指示是否在 Pivot Table 视图的同一列中显示下一个字段的标签。 |
| [getShowInCompactForm()](#getShowInCompactForm--) | 获取一个值，指示此行字段是否使用紧凑形式布局。 |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | 获取一个值，指示此行字段是否使用大纲布局。 |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | 指示是否在项目的顶部或底部显示小计。 |
| [getShowValuesSetting()](#getShowValuesSetting--) | 获取在使用 ShowDataAs 计算时显示值的设置。 |
| [getSortSetting()](#getSortSetting--) | 获取自动排序的所有设置 |
| [getSubtotals()](#getSubtotals--) | 获取字段的小计。 |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | 指示是否显示此透视字段的指定小计。 |
| [getTop10AutoShowSettings()](#getTop10AutoShowSettings--) | 获取透视字段的前 10 项自动显示设置。 |
| [group()](#group--) | 自动对字段进行分组。 |
| [group(PivotFieldGroupOptions options)](#group-com.aspose.cells.PivotFieldGroupOptions-) | 对透视字段进行分组并提供选项。 |
| [groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-) | 按日期分组类型对文件进行分组。 |
| [groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)](#groupBy-boolean-double-boolean-double-double-boolean-) | 按数字对文件进行分组。 |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | 自定义字段分组。 |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | 按日期分组类型对文件进行分组。 |
| [groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-) | 自定义字段分组。 |
| [groupBy(double interval, boolean newField)](#groupBy-double-boolean-) | 使用间隔自动对字段进行分组 |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | 按数字对文件进行分组。 |
| [groupBy(int[] groups, double interval, boolean newField)](#groupBy-int---double-boolean-) | 使用内部自动对字段进行分组 |
| [hashCode()](#hashCode--) |  |
| [hideAllDetails()](#hideAllDetails--) | 隐藏每个透视项的所有详细信息。 |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | 设置是否隐藏透视字段中所有 PivotItems 的详细信息。 |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | 设置数据字段中特定 PivotItem 是否隐藏。 |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | 设置数据字段中特定 PivotItem 是否隐藏。 |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | 设置透视字段中特定 PivotItem 的详细信息是否隐藏。 |
| [initPivotItems()](#initPivotItems--) | 初始化透视字段的透视项 |
| [isAscendShow()](#isAscendShow--) | 指示指定的 PivotTable 字段是否以升序自动显示。 |
| [isAscendSort()](#isAscendSort--) | 指示此透视字段的项是否已自动升序排序。 |
| [isAutoShow()](#isAutoShow--) | 指示指定的 PivotTable 字段是否自动显示。 |
| [isAutoSort()](#isAutoSort--) | 指示此 PivotTable 字段的项是否自动排序。 |
| [isAutoSubtotals()](#isAutoSubtotals--) | 指示指定字段是否显示自动小计。 |
| [isCalculatedField()](#isCalculatedField--) | 指示此透视字段是否为计算字段。 |
| [isHiddenItem(int index)](#isHiddenItem-int-) | 指示特定 PivotItem 是否隐藏。 |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | 指示是否隐藏特定 PivotItem 的详细信息.. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | 指示是否在手动筛选中将新项包含到字段中。 |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | 指示是否在每个项后插入分页符。 |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | 指示是否可以在页面字段中选择多个项。 |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | 指示是否在行或列区域重复字段标签。 |
| [isValueFields()](#isValueFields--) | 指示此字段是否表示值字段。 |
| [isValuesField()](#isValuesField--) | 指示此字段是否表示值字段。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDraggingToColumn(boolean value)](#setAllowDraggingToColumn-boolean-) | 指示指定字段是否可以拖动到列区域。 |
| [setAllowDraggingToData(boolean value)](#setAllowDraggingToData-boolean-) | 指示指定字段是否可以拖动到值区域。 |
| [setAllowDraggingToPage(boolean value)](#setAllowDraggingToPage-boolean-) | 指示指定字段是否可以拖动到页面区域。 |
| [setAllowDraggingToRow(boolean value)](#setAllowDraggingToRow-boolean-) | 指示指定字段是否可以拖动到行区域。 |
| [setAllowRemovingFromView(boolean value)](#setAllowRemovingFromView-boolean-) | 指示是否可以从数据透视表视图中移除此透视字段。 |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | 指示指定的 PivotTable 字段是否以升序自动显示。 |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | 指示此透视字段的项是否已自动升序排序。 |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | 指示指定的 PivotTable 字段是否自动显示。 |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | 表示在指定的 PivotTable 字段中自动显示的前或后项目的数量。 |
| [setAutoShowField(int value)](#setAutoShowField-int-) | 表示自动显示字段索引。-1 表示 PivotField 本身。 |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | 指示此 PivotTable 字段的项是否自动排序。 |
| [setAutoSortField(int value)](#setAutoSortField-int-) | 表示自动排序字段的索引 |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | 指示指定字段是否显示自动小计。 |
| [setBaseIndex(int value)](#setBaseIndex-int-) | 表示源透视字段中的索引。 |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | 设置此透视字段当前显示的页面项（仅限页面字段）。 |
| [setCurrentPageItemText(String value)](#setCurrentPageItemText-java.lang.String-) | 获取此透视字段当前页面项的显示文本（仅限页面字段）。 |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | 表示数据透视表视图中透视字段的显示名称。 |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | 指示指定字段是否可以拖动到列区域。 |
| [setDragToData(boolean value)](#setDragToData-boolean-) | 指示指定字段是否可以拖动到值区域。 |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | 指示是否可以从数据透视表视图中移除此透视字段。 |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | 指示指定字段是否可以拖动到页面区域。 |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | 指示指定字段是否可以拖动到行区域。 |
| [setFunction(int value)](#setFunction-int-) | 表示用于汇总此数据透视表数据字段的函数。 |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | 指示是否在手动筛选中将新项包含到字段中。 |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | 指示是否在每个项目后插入空行。 |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | 指示是否在每个项后插入分页符。 |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | 指示是否可以在页面字段中选择多个项。 |
| [setName(String value)](#setName-java.lang.String-) | 表示 PivotField 的名称。 |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | 指示将应用于此透视字段的排序操作是自动排序还是简单数据排序。 |
| [setNumber(int value)](#setNumber-int-) | 表示数字和日期的内置显示格式。 |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | 表示数字和日期的自定义显示格式。 |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | 指示是否在行或列区域重复字段标签。 |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | 指示是否在 PivotTable 视图中显示所有项目，即使它们不包含汇总数据。 |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | 指示是否在 Pivot Table 视图的同一列中显示下一个字段的标签。 |
| [setShowInCompactForm(boolean value)](#setShowInCompactForm-boolean-) | 设置一个值，指示此行字段是否使用紧凑形式布局。 |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | 设置一个值，指示此行字段是否使用大纲布局。 |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | 指示是否在项目的顶部或底部显示小计。 |
| [setSubtotals(int value)](#setSubtotals-int-) | 设置字段的小计。 |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | 设置指定字段的小计方式。 |
| [showAllDetails()](#showAllDetails--) | 显示每个数据透视项的所有详细信息。 |
| [showValuesAs(int showValuesAsType, int baseField, int baseItem)](#showValuesAs-int-int-int-) | 设置此数据透视字段的“显示值方式”计算。 |
| [showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)](#showValuesAs-int-int-int-int-) | 当使用 ShowDataAs 计算时，以不同的显示格式显示数据字段的值。 |
| [showValuesAs(int showValuesAsType, String baseField, String baseItem)](#showValuesAs-int-java.lang.String-java.lang.String-) | 配置此数据字段的“显示值方式”计算。 |
| [sortBy(int sortType)](#sortBy-int-) | 对该数据透视字段进行排序。 |
| [sortBy(int sortType, int fieldSortedBy)](#sortBy-int-int-) | 对该数据透视字段进行排序。 |
| [sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)](#sortBy-int-int-int-java.lang.String-) | 对该数据透视字段进行排序。 |
| [sortBy(int sortType, int fieldSortedBy, String cellName)](#sortBy-int-int-java.lang.String-) | 对该数据透视字段进行排序。 |
| [toString()](#toString--) |  |
| [top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)](#top10AutoShow-boolean-boolean-int-int-) | 为此数据透视字段配置 Top10 自动显示设置。 |
| [ungroup()](#ungroup--) | 取消对数据透视字段的分组。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


向透视字段添加计算公式项。

**Remarks**

仅支持向行/列字段添加计算项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 该项的名称。 |
| formula | java.lang.String | 数据透视项的公式。 |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


清除此透视字段的筛选设置。

### dispose() {#dispose--}
```
public void dispose()
```


执行应用程序定义的任务，以释放、释放或重置非托管资源。

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
### filterByDate(int type, DateTime dateTime1, DateTime dateTime2) {#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter filterByDate(int type, DateTime dateTime1, DateTime dateTime2)
```


按行或列透视字段的日期值进行筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). 过滤数据的类型。 |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | 过滤条件的日期标签 |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | 介于过滤条件之间的上限日期标签 |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByLabel(int type, String label1, String label2) {#filterByLabel-int-java.lang.String-java.lang.String-}
```
public PivotFilter filterByLabel(int type, String label1, String label2)
```


按行或列透视字段的标题进行筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). 过滤数据的类型。 |
| label1 | java.lang.String | 过滤条件的标签 |
| label2 | java.lang.String | 介于过滤条件之间的上限标签 |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByValue(int valueFieldIndex, int type, double value1, double value2) {#filterByValue-int-int-double-double-}
```
public PivotFilter filterByValue(int valueFieldIndex, int type, double value1, double value2)
```


按数据透视字段的值进行筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| valueFieldIndex | int | 值区域中值字段的索引。 |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). 过滤数据的类型。 |
| value1 | double | 过滤条件的值 |
| value2 | double | 介于过滤条件之间的上限值 |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount) {#filterTop10-int-int-boolean-int-}
```
public PivotFilter filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)
```


按数据透视字段的值进行筛选。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| valueFieldIndex | int | 数据区域中数据字段的索引。 |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). 过滤数据的类型。仅可为 Count、Sum 和 Percent。 |
| isTop | boolean | 指示过滤是来自顶部还是底部 |
| itemCount | int | 项目计数 |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getAllowDraggingToColumn() {#getAllowDraggingToColumn--}
```
public boolean getAllowDraggingToColumn()
```


指示指定字段是否可以拖动到列区域。默认值为 true。

**Returns:**
boolean
### getAllowDraggingToData() {#getAllowDraggingToData--}
```
public boolean getAllowDraggingToData()
```


指示指定字段是否可以拖动到数值区域。默认值为 true。

**Returns:**
boolean
### getAllowDraggingToPage() {#getAllowDraggingToPage--}
```
public boolean getAllowDraggingToPage()
```


指示指定字段是否可以拖动到页面区域。默认值为 true。

**Returns:**
boolean
### getAllowDraggingToRow() {#getAllowDraggingToRow--}
```
public boolean getAllowDraggingToRow()
```


指示指定字段是否可以拖动到行区域。默认值为 true。

**Returns:**
boolean
### getAllowRemovingFromView() {#getAllowRemovingFromView--}
```
public boolean getAllowRemovingFromView()
```


指示此数据透视字段是否可以从数据透视表视图中移除。默认值为 true。

**Returns:**
boolean
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


表示在指定的 PivotTable 字段中自动显示的前或后项目的数量。

**Remarks**

注意：此属性已过时。请改用 PivotField.Top10AutoShowSettings.AutoShowCount 属性或 PivotField.Top10AutoShow() 方法。此方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getAutoShowField() {#getAutoShowField--}
```
public int getAutoShowField()
```


表示自动显示字段的索引。-1 表示 PivotField 本身。它应为数据字段的索引。

**Remarks**

注意：此属性已过时。请改用 PivotField.Top10AutoShowSettings.RankBy 属性或 PivotField.Top10AutoShow() 方法。此方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getAutoSortField() {#getAutoSortField--}
```
public int getAutoSortField()
```


表示自动排序字段的索引。-1 表示 PivotField 本身，其他值表示数据字段的位置。

**Remarks**

注意：此属性已过时。请改用 PivotField.SortSetting.SortBy 属性或 PivotField.SortBy() 方法。此方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


表示源透视字段中的索引。

**Remarks**

注意：此属性的 setter 已过时。此属性的 setter 将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


获取指定计算字段的公式字符串。

**Remarks**

注意：此方法现已过时。请改用 PivotField.GetFormula() 方法。此方法将在自 2024 年 8 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPageItem() {#getCurrentPageItem--}
```
public short getCurrentPageItem()
```


获取此透视字段当前显示的页面项（仅限页面字段）。

**Remarks**

使用 [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) 作为哨兵值以指示“全选”。这是预定义的标记，不是有效的项目索引。

**Returns:**
短
### getCurrentPageItemText() {#getCurrentPageItemText--}
```
public String getCurrentPageItemText()
```


获取此透视字段当前页面项的显示文本（仅限页面字段）。

**Remarks**

当 [getCurrentPageItem()](../../com.aspose.cells/pivotfield\\#getCurrentPageItem--) 等于 [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) 时返回“(All)”。对于其他值，返回项目索引的字符串表示。

**Returns:**
java.lang.String
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


表示数据透视表视图中透视字段的显示名称。

**Returns:**
java.lang.String
### getDragToColumn() {#getDragToColumn--}
```
public boolean getDragToColumn()
```


指示指定字段是否可以拖动到列区域。默认值为 true。

**Remarks**

注意：此属性现已过时。请改用 PivotField.AllowDraggingToColumn 属性。此方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getDragToData() {#getDragToData--}
```
public boolean getDragToData()
```


指示指定字段是否可以拖动到数值区域。默认值为 true。

**Remarks**

注意：此属性现已过时。请改用 PivotField.AllowDraggingToData 属性。此方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


指示此数据透视字段是否可以从数据透视表视图中移除。默认值为 true。

**Remarks**

注意：此属性现已过时。请改用 PivotField.AllowRemovingFromView 属性。此方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getDragToPage() {#getDragToPage--}
```
public boolean getDragToPage()
```


指示指定字段是否可以拖动到页面区域。默认值为 true。

**Remarks**

注意：此属性现已过时。请改用 PivotField.AllowDraggingToPage 属性。此方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getDragToRow() {#getDragToRow--}
```
public boolean getDragToRow()
```


指示指定字段是否可以拖动到行区域。默认值为 true。

**Remarks**

注意：此属性现已过时。请改用 PivotField.AllowDraggingToRow 属性。此方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getFilters() {#getFilters--}
```
public PivotFilter[] getFilters()
```


获取此透视字段应用的所有透视筛选器。

**Returns:**
com.aspose.cells.PivotFilter[]
### getFormula() {#getFormula--}
```
public String getFormula()
```


获取计算字段的公式。仅适用于计算字段。

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


表示用于汇总此数据透视表数据字段的函数。

参见 [ConsolidationFunction](../../com.aspose.cells/consolidationfunction)。

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


获取透视字段的分组设置。

**Remarks**

如果此字段未分组，将返回 Null。

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


指示是否在每个项目后插入空行。仅适用于行字段。

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


获取此透视字段中基础项目的计数。

**Remarks**

注意：此方法现已过时。请改用 PivotField.PivotItems.Count 属性。此方法将在自 2026 年 8 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


获取此字段中透视项目的所有标签。

**Returns:**
java.lang.String[]
### getMaxValue() {#getMaxValue--}
```
public CellValue getMaxValue()
```


获取此字段的最大值。

**Remarks**

仅适用于值必须为日期时间、数字或空白的行或列字段。

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getMinValue() {#getMinValue--}
```
public CellValue getMinValue()
```


获取此字段的最大值。

**Remarks**

仅适用于值必须为日期时间、数字或空白的行或列字段。

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getName() {#getName--}
```
public String getName()
```


表示 PivotField 的名称。

**Returns:**
java.lang.String
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```
public boolean getNonAutoSortDefault()
```


指示将应用于此透视字段的排序操作是自动排序还是简单数据排序。

**Remarks**

注意：此属性现已过时。请改用 !PivotField.SortSetting.IsSimpleSort 属性。此方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getNumber() {#getNumber--}
```
public int getNumber()
```


表示数字和日期的内置显示格式。

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


表示数字和日期的自定义显示格式。

**Returns:**
java.lang.String
### getOriginalItems() {#getOriginalItems--}
```
public String[] getOriginalItems()
```


获取原始基础项目；

**Returns:**
java.lang.String[]
### getPivotFilterByType(int type) {#getPivotFilterByType-int-}
```
public PivotFilter getPivotFilterByType(int type)
```


获取按类型划分的透视字段的透视过滤器

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 类型 | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getPivotFilters() {#getPivotFilters--}
```
public ArrayList getPivotFilters()
```


获取透视字段的透视过滤器

**Remarks**

注意：此方法现已过时。请改用 PivotField.GetFilters() 方法。此方法将在自 2023 年 11 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.util.ArrayList
### getPivotItems() {#getPivotItems--}
```
public PivotItemCollection getPivotItems()
```


获取透视字段的透视项目

**Returns:**
[PivotItemCollection](../../com.aspose.cells/pivotitemcollection)
### getPosition() {#getPosition--}
```
public int getPosition()
```


表示区域中 [PivotField](../../com.aspose.cells/pivotfield) 的索引。

**Returns:**
int
### getRegionType() {#getRegionType--}
```
public int getRegionType()
```


指定此字段显示的透视表区域。

请参阅 [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。

**Returns:**
int
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


指示是否在 PivotTable 视图中显示所有项目，即使它们不包含汇总数据。默认值为 false。

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


指示是否在 Pivot Table 视图的同一列中显示下一个字段的标签。仅适用于行字段。

**Remarks**

注意：此方法现已过时。请改用 PivotField.ShowInCompactForm 属性。此方法将在自 2026 年 11 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getShowInCompactForm() {#getShowInCompactForm--}
```
public boolean getShowInCompactForm()
```


获取一个值，指示此行字段是否使用紧凑形式布局。仅适用于行字段。

**Remarks**

紧凑形式是大纲布局的子模式。仅当 [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\\#getShowInOutlineForm--) 为 true 时，此设置才生效。

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


获取一个值，指示此行字段是否使用大纲布局。仅适用于行字段。

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


指示是否在项目的顶部或底部显示小计。

**Remarks**

仅在 ShowInOutlineForm 为 true 时适用于行区域中的透视字段。

**Returns:**
boolean
### getShowValuesSetting() {#getShowValuesSetting--}
```
public PivotShowValuesSetting getShowValuesSetting()
```


获取在使用 ShowDataAs 计算时显示值的设置。

**Returns:**
[PivotShowValuesSetting](../../com.aspose.cells/pivotshowvaluessetting)
### getSortSetting() {#getSortSetting--}
```
public PivotFieldSortSetting getSortSetting()
```


获取自动排序的所有设置

**Returns:**
[PivotFieldSortSetting](../../com.aspose.cells/pivotfieldsortsetting)
### getSubtotals() {#getSubtotals--}
```
public int getSubtotals()
```


获取字段的小计。仅适用于行或列透视字段。

查看 [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)。

**Example**

```
         //No subtotals
         rowField.setSubtotals(PivotFieldSubtotalType.NONE);
         //Automatic subtotals
         //rowField.Subtotals = PivotFieldSubtotalType.Automatic;
         //Single subtotals: Sum
         //rowField.Subtotals = PivotFieldSubtotalType.Sum;
         //Multipl subtotals: Sum and count numbers 
         //rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

**Returns:**
int
### getSubtotals(int subtotalType) {#getSubtotals-int-}
```
public boolean getSubtotals(int subtotalType)
```


指示是否显示此透视字段的指定小计。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)。小计类型。 |

**Returns:**
boolean - 返回是否显示指定的小计。
### getTop10AutoShowSettings() {#getTop10AutoShowSettings--}
```
public PivotFieldTop10AutoShowSettings getTop10AutoShowSettings()
```


获取透视字段的前 10 项自动显示设置。

**Returns:**
[PivotFieldTop10AutoShowSettings](../../com.aspose.cells/pivotfieldtop10autoshowsettings)
### group() {#group--}
```
public boolean group()
```


自动对字段进行分组。

**Remarks**

如果字段仅包含空值和日期时间，则字段将按月份分组。如果字段仅包含空值和数字，则字段将按数字分组。否则仅返回 false，且不进行任何分组。

**Returns:**
boolean
### group(PivotFieldGroupOptions options) {#group-com.aspose.cells.PivotFieldGroupOptions-}
```
public boolean group(PivotFieldGroupOptions options)
```


对透视字段进行分组并提供选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [PivotFieldGroupOptions](../../com.aspose.cells/pivotfieldgroupoptions) | 用于数据透视字段分组设置的选项。 |

**Returns:**
boolean -
### groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


按日期分组类型对文件进行分组。

**Remarks**

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isAutoStart | boolean | 指示是否自动检测开始日期时间值。 |
| start | [DateTime](../../com.aspose.cells/datetime) | 开始日期时间 |
| isAutoEnd | boolean | 指示是否自动检测结束日期时间值。 |
| end | [DateTime](../../com.aspose.cells/datetime) | 结束日期时间 |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype)。分组类型 |
| interval | double | 间隔 |
| firstAsNewField | boolean | 指示是否向数据透视表添加新字段。仅适用于第一个分组项。 |

**Returns:**
boolean - False 表示此字段无法按日期时间分组。
### groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField) {#groupBy-boolean-double-boolean-double-double-boolean-}
```
public boolean groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)
```


按数字对文件进行分组。

**Remarks**

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isAutoStart | boolean | 指示是否自动检测起始值。 |
| start | double | 起始值 |
| isAutoEnd | boolean | 指示是否自动检测结束值。 |
| end | double | 结束值 |
| interval | double | 间隔 |
| newField | boolean | 指示是否向数据透视表添加新字段 |

**Returns:**
boolean - False 表示此字段无法按日期时间分组。
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public boolean groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


自定义字段分组。

**Remarks**

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions options) 方法，并使用 PivotFieldGroupOptions.DiscreteGroupItems 属性。此方法将在 2026 年 7 月起 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | 自定义分组项。 |
| newField | boolean | 指示是否向数据透视表添加新字段 |

**Returns:**
boolean - False 表示此字段无法按日期时间分组。
### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


按日期分组类型对文件进行分组。

**Remarks**

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | 开始日期时间 |
| end | [DateTime](../../com.aspose.cells/datetime) | 结束日期时间 |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype)。分组类型 |
| interval | double | 间隔 |
| firstAsNewField | boolean | 指示是否向数据透视表添加新字段。仅适用于第一个分组项。 |

**Returns:**
boolean - False 表示此字段无法按日期时间分组。
### groupBy(DiscreteGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-}
```
public boolean groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)
```


自定义字段分组。

**Remarks**

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions options) 方法，并使用 PivotFieldGroupOptions.DiscreteGroupItems 属性。此方法将在 2026 年 7 月起 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| customGroupItems | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) | 自定义分组项。 |
| newField | boolean | 指示是否向数据透视表添加新字段 |

**Returns:**
boolean -
### groupBy(double interval, boolean newField) {#groupBy-double-boolean-}
```
public void groupBy(double interval, boolean newField)
```


使用间隔自动对字段进行分组

**Remarks**

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| interval | double | 组的内部。如果为零，将自动分配值， |
| newField | boolean | 指示是否向数据透视表添加新字段。仅适用于 DateTime 分组。 |

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public boolean groupBy(double start, double end, double interval, boolean newField)
```


按数字对文件进行分组。

**Remarks**

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| start | double | 起始值 |
| end | double | 结束值 |
| interval | double | 间隔 |
| newField | boolean | 指示是否向数据透视表添加新字段 |

**Returns:**
boolean - False 表示此字段无法按日期时间分组。
### groupBy(int[] groups, double interval, boolean newField) {#groupBy-int---double-boolean-}
```
public void groupBy(int[] groups, double interval, boolean newField)
```


使用内部自动对字段进行分组

**Remarks**

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype)。分组类型 |
| interval | double | 组的内部。如果为零，将自动分配值，仅适用于按数字或天数进行分组。 |
| newField | boolean | 指示是否向数据透视表添加新字段。 |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideAllDetails() {#hideAllDetails--}
```
public void hideAllDetails()
```


隐藏每个透视项的所有详细信息。

### hideDetail(boolean isHiddenDetail) {#hideDetail-boolean-}
```
public void hideDetail(boolean isHiddenDetail)
```


设置是否隐藏透视字段中所有 PivotItems 的详细信息。即折叠/展开此字段。

**Remarks**

注意：此方法现已过时。请改用 PivotItemsCollection.HideAllDetails() 和 UnhideAllDetails() 方法。此方法将在 2026 年 11 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isHiddenDetail | boolean | 是否隐藏透视字段的细节。 |

### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


设置数据字段中特定 PivotItem 是否隐藏。

**Remarks**

注意：此方法现已过时。请改用 PivotField.PivotItems[int].IsHidden 属性。此方法将在 2026 年 8 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | pivotField 中 pivotItem 的索引。 |
| isHidden | boolean | 特定 PivotItem 是否隐藏 |

### hideItem(String itemValue, boolean isHidden) {#hideItem-java.lang.String-boolean-}
```
public void hideItem(String itemValue, boolean isHidden)
```


设置数据字段中特定 PivotItem 是否隐藏。

**Remarks**

注意：此方法现已过时。请改用 PivotField.PivotItems[string].IsHidden 属性。此方法将在 2026 年 8 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| itemValue | java.lang.String | pivotField 中 pivotItem 的名称。 |
| isHidden | boolean | 特定 PivotItem 是否隐藏 |

### hideItemDetail(int index, boolean isHiddenDetail) {#hideItemDetail-int-boolean-}
```
public void hideItemDetail(int index, boolean isHiddenDetail)
```


设置透视字段中特定 PivotItem 的详细信息是否隐藏。

**Remarks**

注意：此方法现已过时。请改用 PivotField.PivotItems[int].IsDetailHidden 属性。此方法将在 2026 年 8 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | pivotField 中 pivotItem 的索引。 |
| isHiddenDetail | boolean | 特定 PivotItem 是否隐藏 |

### initPivotItems() {#initPivotItems--}
```
public void initPivotItems()
```


初始化透视字段的透视项

**Remarks**

注意：此方法现已过时。请直接删除对该方法的调用。此方法将在 2026 年 10 月起 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### isAscendShow() {#isAscendShow--}
```
public boolean isAscendShow()
```


指示指定的 PivotTable 字段是否以升序自动显示。

**Remarks**

注意：此属性现已过时。请改用 PivotField.Top10AutoShowSettings.IsTop 属性或 PivotField.Top10AutoShow() 方法。此方法将在 2026 年 9 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


指示此透视字段的项是否已自动升序排序。

**Remarks**

注意：此属性现已过时。请改用 PivotField.SortSetting.SortType 属性或 PivotField.SortBy() 方法。此方法将在 2026 年 9 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


指示指定的 PivotTable 字段是否自动显示。

**Remarks**

注意：此属性现已过时。请改用 PivotField.Top10AutoShowSettings.IsAutoShow 属性或 PivotField.Top10AutoShow() 方法。此方法将在 2026 年 9 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


指示此 PivotTable 字段的项是否自动排序。

**Remarks**

注意：此属性现已过时。请改用 PivotField.SortSetting.SortType 属性或 PivotField.SortBy() 方法。此方法将在 2026 年 9 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### isAutoSubtotals() {#isAutoSubtotals--}
```
public boolean isAutoSubtotals()
```


指示指定字段是否显示自动小计。默认值为 true。

**Returns:**
boolean
### isCalculatedField() {#isCalculatedField--}
```
public boolean isCalculatedField()
```


指示此透视字段是否为计算字段。

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


指示特定 PivotItem 是否隐藏。

**Remarks**

注意：此方法现已过时。请改用 PivotField.PivotItems[int].IsHidden 属性。此方法将在 2026 年 8 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | pivotField 中 pivotItem 的索引。 |

**Returns:**
布尔值 - 特定 PivotItem 是否隐藏
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


指示是否隐藏特定 PivotItem 的详细信息..

**Remarks**

注意：此方法现已过时。请改用 PivotField.PivotItems[int].IsDetailHidden 属性。此方法将在 2026 年 8 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | pivotField 中 pivotItem 的索引。 |

**Returns:**
布尔值 - 特定 PivotItem 的隐藏细节
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


指示是否在手动筛选中将新项目包含到字段中。默认值为 false。

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


指示是否在每个项目后插入分页符。默认值为 false。

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


指示页面字段是否可以选择多个项目。默认值为 false。

**Remarks**

仅适用于页面（筛选）字段。

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


指示是否在行或列区域重复该字段的标签。默认值为 false。

**Returns:**
boolean
### isValueFields() {#isValueFields--}
```
public boolean isValueFields()
```


指示此字段是否表示值字段。

**Remarks**

注意：此方法现已过时。请改用 PivotField.IsValuesField 属性。此方法将在自 2023 年 11 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### isValuesField() {#isValuesField--}
```
public boolean isValuesField()
```


指示此字段是否表示值字段。

**Remarks**

仅在透视表视图中有两个或更多数据字段时有效。

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




### setAllowDraggingToColumn(boolean value) {#setAllowDraggingToColumn-boolean-}
```
public void setAllowDraggingToColumn(boolean value)
```


指示指定字段是否可以拖动到列区域。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowDraggingToData(boolean value) {#setAllowDraggingToData-boolean-}
```
public void setAllowDraggingToData(boolean value)
```


指示指定字段是否可以拖动到数值区域。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowDraggingToPage(boolean value) {#setAllowDraggingToPage-boolean-}
```
public void setAllowDraggingToPage(boolean value)
```


指示指定字段是否可以拖动到页面区域。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowDraggingToRow(boolean value) {#setAllowDraggingToRow-boolean-}
```
public void setAllowDraggingToRow(boolean value)
```


指示指定字段是否可以拖动到行区域。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowRemovingFromView(boolean value) {#setAllowRemovingFromView-boolean-}
```
public void setAllowRemovingFromView(boolean value)
```


指示此数据透视字段是否可以从数据透视表视图中移除。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAscendShow(boolean value) {#setAscendShow-boolean-}
```
public void setAscendShow(boolean value)
```


指示指定的 PivotTable 字段是否以升序自动显示。

**Remarks**

注意：此属性现已过时。请改用 PivotField.Top10AutoShowSettings.IsTop 属性或 PivotField.Top10AutoShow() 方法。此方法将在 2026 年 9 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


指示此透视字段的项是否已自动升序排序。

**Remarks**

注意：此属性现已过时。请改用 PivotField.SortSetting.SortType 属性或 PivotField.SortBy() 方法。此方法将在 2026 年 9 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


指示指定的 PivotTable 字段是否自动显示。

**Remarks**

注意：此属性现已过时。请改用 PivotField.Top10AutoShowSettings.IsAutoShow 属性或 PivotField.Top10AutoShow() 方法。此方法将在 2026 年 9 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


表示在指定的 PivotTable 字段中自动显示的前或后项目的数量。

**Remarks**

注意：此属性已过时。请改用 PivotField.Top10AutoShowSettings.AutoShowCount 属性或 PivotField.Top10AutoShow() 方法。此方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


表示自动显示字段的索引。-1 表示 PivotField 本身。它应为数据字段的索引。

**Remarks**

注意：此属性已过时。请改用 PivotField.Top10AutoShowSettings.RankBy 属性或 PivotField.Top10AutoShow() 方法。此方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


指示此 PivotTable 字段的项是否自动排序。

**Remarks**

注意：此属性现已过时。请改用 PivotField.SortSetting.SortType 属性或 PivotField.SortBy() 方法。此方法将在 2026 年 9 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


表示自动排序字段的索引。-1 表示 PivotField 本身，其他值表示数据字段的位置。

**Remarks**

注意：此属性已过时。请改用 PivotField.SortSetting.SortBy 属性或 PivotField.SortBy() 方法。此方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


指示指定字段是否显示自动小计。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


表示源透视字段中的索引。

**Remarks**

注意：此属性的 setter 已过时。此属性的 setter 将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


设置此透视字段当前显示的页面项（仅限页面字段）。

**Remarks**

使用 [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) 作为哨兵值以指示“全选”。这是预定义的标记，不是有效的项目索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 短 |  |

### setCurrentPageItemText(String value) {#setCurrentPageItemText-java.lang.String-}
```
public void setCurrentPageItemText(String value)
```


获取此透视字段当前页面项的显示文本（仅限页面字段）。

**Remarks**

当 [getCurrentPageItem()](../../com.aspose.cells/pivotfield\\#getCurrentPageItem--) 等于 [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) 时返回“(All)”。对于其他值，返回项目索引的字符串表示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


表示数据透视表视图中透视字段的显示名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


指示指定字段是否可以拖动到列区域。默认值为 true。

**Remarks**

注意：此属性现已过时。请改用 PivotField.AllowDraggingToColumn 属性。此方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


指示指定字段是否可以拖动到数值区域。默认值为 true。

**Remarks**

注意：此属性现已过时。请改用 PivotField.AllowDraggingToData 属性。此方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


指示此数据透视字段是否可以从数据透视表视图中移除。默认值为 true。

**Remarks**

注意：此属性现已过时。请改用 PivotField.AllowRemovingFromView 属性。此方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


指示指定字段是否可以拖动到页面区域。默认值为 true。

**Remarks**

注意：此属性现已过时。请改用 PivotField.AllowDraggingToPage 属性。此方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


指示指定字段是否可以拖动到行区域。默认值为 true。

**Remarks**

注意：此属性现已过时。请改用 PivotField.AllowDraggingToRow 属性。此方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


表示用于汇总此数据透视表数据字段的函数。

参见 [ConsolidationFunction](../../com.aspose.cells/consolidationfunction)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


指示是否在手动筛选中将新项目包含到字段中。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


指示是否在每个项目后插入空行。仅适用于行字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


指示是否在每个项目后插入分页符。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


指示页面字段是否可以选择多个项目。默认值为 false。

**Remarks**

仅适用于页面（筛选）字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


表示 PivotField 的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


指示将应用于此透视字段的排序操作是自动排序还是简单数据排序。

**Remarks**

注意：此属性现已过时。请改用 !PivotField.SortSetting.IsSimpleSort 属性。此方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


表示数字和日期的内置显示格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


表示数字和日期的自定义显示格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


指示是否在行或列区域重复该字段的标签。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


指示是否在 PivotTable 视图中显示所有项目，即使它们不包含汇总数据。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


指示是否在 Pivot Table 视图的同一列中显示下一个字段的标签。仅适用于行字段。

**Remarks**

注意：此方法现已过时。请改用 PivotField.ShowInCompactForm 属性。此方法将在自 2026 年 11 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowInCompactForm(boolean value) {#setShowInCompactForm-boolean-}
```
public void setShowInCompactForm(boolean value)
```


设置一个值，指示此行字段是否使用紧凑形式布局。仅适用于行字段。

**Remarks**

紧凑形式是大纲布局的子模式。仅当 [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\\#getShowInOutlineForm--) 为 true 时，此设置才生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


设置一个值，指示此行字段是否使用大纲布局。仅适用于行字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


指示是否在项目的顶部或底部显示小计。

**Remarks**

仅在 ShowInOutlineForm 为 true 时适用于行区域中的透视字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSubtotals(int value) {#setSubtotals-int-}
```
public void setSubtotals(int value)
```


设置字段的小计。仅适用于行或列透视字段。

查看 [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


设置指定字段的小计方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| 显示 | boolean | 指定字段是否显示小计。 |

### showAllDetails() {#showAllDetails--}
```
public void showAllDetails()
```


显示每个数据透视项的所有详细信息。

### showValuesAs(int showValuesAsType, int baseField, int baseItem) {#showValuesAs-int-int-int-}
```
public void showValuesAs(int showValuesAsType, int baseField, int baseItem)
```


设置此数据透视字段的“显示值方式”计算。

**Remarks**

仅适用于数据字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype)。"Show Values As" 计算的类型。 |
| baseField | int | 用于计算的基字段索引。 |
| baseItem | int | 用于计算的基项索引。使用 [PivotShowValuesSetting.PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) 表示前一个项，使用 [PivotShowValuesSetting.NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) 表示后一个项；non\\u9225\\u6182egative 值表示特定透视项的序数索引。 |

### showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem) {#showValuesAs-int-int-int-int-}
```
public void showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)
```


当使用 ShowDataAs 计算时，以不同的显示格式显示数据字段的值。

**Remarks**

注意：此属性现已过时。请改用 PivotField.ShowValuesAs(PivotShowValuesAsType,int,int) 方法。此方法将在自 2026 年 11 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| displayFormat | int | [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat)。数据显示格式类型。 |
| baseField | int | 用于 ShowDataAs 计算的字段索引。 |
| baseItemPositionType | int | [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype)。基项的定位类型。 |
| baseItem | int | 用于 ShowDataAs 计算的基项索引。仅在 baseItemPositionType 为 custom 时有效。 |

### showValuesAs(int showValuesAsType, String baseField, String baseItem) {#showValuesAs-int-java.lang.String-java.lang.String-}
```
public void showValuesAs(int showValuesAsType, String baseField, String baseItem)
```


配置此数据字段的“显示值方式”计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype)。Show Values As 的计算类型。 |
| baseField | java.lang.String | 用于计算的基字段名称。 |
| baseItem | java.lang.String | 常规透视项的标题。还接受保留文字关键字：`(previous)` 表示前一个项，`(next)` 表示下一个项。如果所选计算类型不需要基项，请传入 `null`。 |

### sortBy(int sortType) {#sortBy-int-}
```
public void sortBy(int sortType)
```


对该数据透视字段进行排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder)。此字段的排序类型。 |

### sortBy(int sortType, int fieldSortedBy) {#sortBy-int-int-}
```
public void sortBy(int sortType, int fieldSortedBy)
```


对该数据透视字段进行排序。

**Remarks**

注意：此属性已过时。请改用 PivotField.SortBy(SortOrder, int,string) 方法或 PivotField.IsAutoSort 属性。此方法将在自2026年9月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder)。此字段的排序类型。 |
| fieldSortedBy | int | 按此进行排序的透视字段的索引。-1 表示按该字段的数据标签排序，其他值表示按相应数据字段的索引排序。 |

### sortBy(int sortType, int fieldSortedBy, int dataType, String cellName) {#sortBy-int-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)
```


对该数据透视字段进行排序。

**Remarks**

注意：此属性已过时。请改用 PivotField.SortBy(SortOrder, int,string) 方法。此方法将在自2026年9月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder)。此字段的排序类型。 |
| fieldSortedBy | int | 按此进行排序的透视字段的索引。-1 表示按该字段的数据标签排序，其他值表示按相应数据字段的索引排序。 |
| dataType | int | [PivotLineType](../../com.aspose.cells/pivotlinetype)。排序数据的类型。 |
| cellName | java.lang.String | 按行或列的值排序 |

### sortBy(int sortType, int fieldSortedBy, String cellName) {#sortBy-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, String cellName)
```


对该数据透视字段进行排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder)。此字段的排序类型。 |
| fieldSortedBy | int | 按此进行排序的透视字段的索引。-1 表示按该字段的数据标签排序，其他值表示按相应数据字段的索引排序。 |
| cellName | java.lang.String | 按行或列的值排序。如果为 Null，则按字段的总计分组，否则按所选列或行的值分组。 |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy) {#top10AutoShow-boolean-boolean-int-int-}
```
public void top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)
```


为此数据透视字段配置 Top10 自动显示设置。

**Remarks**

此方法配置 . XLS 二进制格式：AutoShow（Top10）是原生且唯一支持的选项。XLSX（OpenXML）：底层文件格式支持 Top10 AutoShow，但 Excel 2007 及更高版本的用户界面仅通过 Top10 筛选器公开此功能。如果不需要 XLS 兼容性，建议改用 Top10 筛选器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isAutoShow | boolean | true 表示启用 AutoShow；false 表示禁用。 |
| isTop | boolean | 如果为 true，则显示顶部项目；false 则显示底部项目。 |
| 计数 | int | 要显示的顶部/底部项目数量。 |
| rankBy | int | 用于排名的数据字段索引。使用 -1 可按透视项自身的值进行排名。 |

### ungroup() {#ungroup--}
```
public void ungroup()
```


取消对数据透视字段的分组。

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

