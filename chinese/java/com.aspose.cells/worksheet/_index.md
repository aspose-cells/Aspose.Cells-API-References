---
title: "Worksheet"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示单个工作表的对象。"
type: docs
url: /zh/java/com.aspose.cells/worksheet/
---

**Inheritance:**
java.lang.Object
```
public class Worksheet
```

封装表示单个工作表的对象。

**Example**

以下示例展示了如何使用 .Net 或 VB 冻结窗格并向工作表插入超链接。

```
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Freeze panes at "AS40" with 10 rows and 10 columns
         sheet.freezePanes("AS40", 10, 10);
 
         //Add a hyperlink in Cell A1
         sheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addPageBreaks(String cellName)](#addPageBreaks-java.lang.String-) | 添加分页符。 |
| [advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)](#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-) | 使用复杂条件过滤数据。 |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | 自动调整列宽。 |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | 自动调整列宽。 |
| [autoFitColumns()](#autoFitColumns--) | 自动调整此工作表中所有列的宽度。 |
| [autoFitColumns(AutoFitterOptions options)](#autoFitColumns-com.aspose.cells.AutoFitterOptions-) | 自动调整此工作表中所有列的宽度。 |
| [autoFitColumns(int firstColumn, int lastColumn)](#autoFitColumns-int-int-) | 自动调整列的宽度。 |
| [autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-) | 自动调整列的宽度。 |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)](#autoFitColumns-int-int-int-int-) | 自动调整列的宽度。 |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-) | 自动调整列的宽度。 |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | 自动调整行高。 |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | 自动调整行高。 |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-) | 自动调整行高。 |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | 在矩形范围内自动调整行高。 |
| [autoFitRows()](#autoFitRows--) | 自动调整此工作表中所有行的高度。 |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | 自动调整此工作表中所有行的高度。 |
| [autoFitRows(AutoFitterOptions options)](#autoFitRows-com.aspose.cells.AutoFitterOptions-) | 自动调整此工作表中所有行的高度。 |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | 在范围内自动调整行高。 |
| [autoFitRows(int startRow, int endRow, AutoFitterOptions options)](#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-) | 在范围内自动调整行高。 |
| [calculateArrayFormula(String formula, CalculationOptions opts)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | 将公式计算为数组公式。 |
| [calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-) | 将公式计算为数组公式。 |
| [calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)](#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-) | 将公式计算为数组公式。 |
| [calculateFormula(CalculationOptions options, boolean recursive)](#calculateFormula-com.aspose.cells.CalculationOptions-boolean-) | 计算此工作表中的所有公式。 |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | 计算一个公式。 |
| [calculateFormula(String formula, CalculationOptions opts)](#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | 直接计算公式表达式。 |
| [calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)](#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-) | 直接计算公式表达式。 |
| [clearComments()](#clearComments--) | 清除设计器电子表格中的所有批注。 |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | 关闭使用缓存访问此工作表数据的会话。 |
| [convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)](#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-) | 转换公式引用样式。 |
| [copy(Worksheet sourceSheet)](#copy-com.aspose.cells.Worksheet-) | 复制来自另一个工作表的内容和格式。 |
| [copy(Worksheet sourceSheet, CopyOptions copyOptions)](#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-) | 复制来自另一个工作表的内容和格式。 |
| [dispose()](#dispose--) | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(CellArea ca)](#filter-com.aspose.cells.CellArea-) | 筛选该范围。 |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | 在工作表中指定的单元格处冻结窗格。 |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | 在工作表中指定的单元格处冻结窗格。 |
| [getActiveCell()](#getActiveCell--) | 获取工作表中的活动单元格。 |
| [getAdvancedFilter()](#getAdvancedFilter--) | 获取高级筛选的设置。 |
| [getAllPictures()](#getAllPictures--) | 获取所有图片，包括嵌入单元格以及位于单元格上方的图像。 |
| [getAllowEditRanges()](#getAllowEditRanges--) | 获取工作表中允许编辑范围的集合。 |
| [getAreasOfXmlMapQuery(String path, XmlMap xmlMap)](#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | 查询映射/链接到特定 XML 映射路径的单元格区域。 |
| [getAutoFilter()](#getAutoFilter--) | 表示指定工作表的自动筛选。 |
| [getBackgroundImage()](#getBackgroundImage--) | 获取工作表的背景图像。 |
| [getCellWatches()](#getCellWatches--) | 获取此工作表在“监视窗口”中被监视的单元格集合。 |
| [getCells()](#getCells--) | 获取 [Cells](../../com.aspose.cells/cells) 集合。 |
| [getCharts()](#getCharts--) | 获取 [Chart](../../com.aspose.cells/chart) 集合 |
| [getCheckBoxes()](#getCheckBoxes--) | 获取 [CheckBox](../../com.aspose.cells/checkbox) 集合。 |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | 获取工作表代码名称。 |
| [getComments()](#getComments--) | 获取 [Comment](../../com.aspose.cells/comment) 集合。 |
| [getConditionalFormattings()](#getConditionalFormattings--) | 获取工作表中的 ConditionalFormattings。 |
| [getCustomProperties()](#getCustomProperties--) | 获取表示与工作表关联的标识信息的对象。 |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | 指示指定的工作表是从右向左显示还是从左向右显示。 |
| [getDisplayZeros()](#getDisplayZeros--) | 如果显示零值，则为 True。 |
| [getErrorCheckOptions()](#getErrorCheckOptions--) | 获取在特定范围上应用的错误检查设置。 |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | 表示第一个可见列的索引。 |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | 表示第一个可见行的索引。 |
| [getFreezedPanes()](#getFreezedPanes--) | 获取冻结窗格。 |
| [getGridlineColor()](#getGridlineColor--) | 获取网格线的颜色 |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | 获取 [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection) 集合。 |
| [getHyperlinks()](#getHyperlinks--) | 获取 [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection) 集合。 |
| [getIndex()](#getIndex--) | 获取工作表集合中工作表的索引。 |
| [getListObjects()](#getListObjects--) | 获取此工作表中的所有 ListObjects。 |
| [getName()](#getName--) | 获取工作表的名称。 |
| [getOleObjects()](#getOleObjects--) | 表示工作表中 [OleObject](../../com.aspose.cells/oleobject) 的集合。 |
| [getOutline()](#getOutline--) | 获取此工作表上的大纲。 |
| [getPageSetup()](#getPageSetup--) | 表示此工作表中的页面设置描述。 |
| [getPaneState()](#getPaneState--) | 指示窗格是否具有水平或垂直拆分，以及这些拆分是否已冻结。 |
| [getPanes()](#getPanes--) | 获取窗口窗格。 |
| [getPictures()](#getPictures--) | 获取 [Picture](../../com.aspose.cells/picture) 集合。 |
| [getPivotTables()](#getPivotTables--) | 获取此工作表中的所有数据透视表。 |
| [getPrintingPageBreaks(ImageOrPrintOptions options)](#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-) | 获取自动分页符。 |
| [getProtection()](#getProtection--) | 表示工作表可用的各种保护选项类型。 |
| [getQueryTables()](#getQueryTables--) | 获取工作表中的 [QueryTableCollection](../../com.aspose.cells/querytablecollection)。 |
| [getScenarios()](#getScenarios--) | 获取 [Scenario](../../com.aspose.cells/scenario) 的集合。 |
| [getSelectedAreas()](#getSelectedAreas--) | 获取设计器电子表格中选定的单元格范围。 |
| [getSelectedRanges()](#getSelectedRanges--) | 获取设计器电子表格中选定的单元格范围。 |
| [getShapes()](#getShapes--) | 返回此工作表中的所有绘图形状。 |
| [getShowDataTypeIcons()](#getShowDataTypeIcons--) | 指示是否显示数据类型图标。 |
| [getShowFormulas()](#getShowFormulas--) | 指示是否显示公式或其结果。 |
| [getSlicers()](#getSlicers--) | 获取工作表中的 Slicer 集合 |
| [getSmartTagSetting()](#getSmartTagSetting--) | 获取工作表的所有 [SmartTagCollection](../../com.aspose.cells/smarttagcollection) 对象。 |
| [getSparklineGroups()](#getSparklineGroups--) | 获取工作表中的 sparkline 组。 |
| [getTabColor()](#getTabColor--) | 表示工作表选项卡颜色。 |
| [getTabId()](#getTabId--) | 指定工作表的内部标识符。 |
| [getTextBoxes()](#getTextBoxes--) | 获取一个 [TextBox](../../com.aspose.cells/textbox) 集合。 |
| [getTimelines()](#getTimelines--) | 获取工作表中的 Timeline 集合 |
| [getTransitionEntry()](#getTransitionEntry--) | 指示是否启用了 Transition Formula Entry（Lotus 兼容）选项。 |
| [getTransitionEvaluation()](#getTransitionEvaluation--) | 指示是否启用了 Transition Formula Evaluation（Lotus 兼容）选项。 |
| [getType()](#getType--) | 表示工作表类型。 |
| [getUniqueId()](#getUniqueId--) | 获取唯一 ID，它与 \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\} 相同。 |
| [getValidations()](#getValidations--) | 获取工作表中的数据验证设置集合。 |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--) | 获取 [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection) 集合。 |
| [getViewType()](#getViewType--) | 获取视图类型。 |
| [getVisibilityType()](#getVisibilityType--) | 指示此工作表的可见状态。 |
| [getWorkbook()](#getWorkbook--) | 获取包含此工作表的工作簿对象。 |
| [getZoom()](#getZoom--) | 表示以百分比计的缩放因子。 |
| [hasAutofilter()](#hasAutofilter--) | 指示此工作表是否具有自动筛选。 |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | 获取一个值，指示网格线是否可见。默认值为 true。 |
| [isOutlineShown()](#isOutlineShown--) | 指示是否显示大纲。 |
| [isPageBreakPreview()](#isPageBreakPreview--) | 指示指定的工作表是以普通视图还是分页预览方式显示。 |
| [isProtected()](#isProtected--) | 指示工作表是否受保护。 |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--) | 获取一个值，指示工作表是否显示行和列标题。 |
| [isRulerVisible()](#isRulerVisible--) | 指示标尺是否可见。 |
| [isSelected()](#isSelected--) | 指示打开工作簿时是否选中此工作表。 |
| [isVisible()](#isVisible--) | 表示工作表是否可见。 |
| [moveTo(int index)](#moveTo-int-) | 将工作表移动到电子表格中的其他位置。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(int type)](#protect-int-) | 保护工作表。 |
| [protect(int type, String password, String oldPassword)](#protect-int-java.lang.String-java.lang.String-) | 保护工作表。 |
| [refreshPivotTables()](#refreshPivotTables--) | 刷新此工作表中的所有数据透视表。 |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | 刷新此工作表中的所有数据透视表。 |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--) | 删除此工作表中的所有绘图对象。 |
| [removeAutoFilter()](#removeAutoFilter--) | 移除工作表的自动筛选。 |
| [removeSplit()](#removeSplit--) | 移除拆分窗口。 |
| [replace(String oldString, String newString)](#replace-java.lang.String-java.lang.String-) | 将所有单元格的文本替换为新字符串。 |
| [selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)](#selectRange-int-int-int-int-boolean-) | 选择一个范围。 |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | 设置工作表中的活动单元格。 |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | 设置工作表的背景图像。 |
| [setCodeName(String value)](#setCodeName-java.lang.String-) | 获取工作表代码名称。 |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | 指示指定的工作表是从右向左显示还是从左向右显示。 |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | 如果显示零值，则为 True。 |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | 表示第一个可见列的索引。 |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | 表示第一个可见行的索引。 |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | 设置网格线的颜色 |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | 设置一个值，指示网格线是否可见。默认值为 true。 |
| [setName(String value)](#setName-java.lang.String-) | 设置工作表的名称。 |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | 指示是否显示大纲。 |
| [setPageBreakPreview(boolean value)](#setPageBreakPreview-boolean-) | 指示指定的工作表是以普通视图还是分页预览方式显示。 |
| [setRowColumnHeadersVisible(boolean value)](#setRowColumnHeadersVisible-boolean-) | 设置一个值，指示工作表是否显示行和列标题。 |
| [setRulerVisible(boolean value)](#setRulerVisible-boolean-) | 指示标尺是否可见。 |
| [setSelected(boolean value)](#setSelected-boolean-) | 指示打开工作簿时是否选中此工作表。 |
| [setShowDataTypeIcons(boolean value)](#setShowDataTypeIcons-boolean-) | 指示是否显示数据类型图标。 |
| [setShowFormulas(boolean value)](#setShowFormulas-boolean-) | 指示是否显示公式或其结果。 |
| [setTabColor(Color value)](#setTabColor-com.aspose.cells.Color-) | 表示工作表选项卡颜色。 |
| [setTabId(int value)](#setTabId-int-) | 指定工作表的内部标识符。 |
| [setTransitionEntry(boolean value)](#setTransitionEntry-boolean-) | 指示是否启用了 Transition Formula Entry（Lotus 兼容）选项。 |
| [setTransitionEvaluation(boolean value)](#setTransitionEvaluation-boolean-) | 指示是否启用了 Transition Formula Evaluation（Lotus 兼容）选项。 |
| [setType(int value)](#setType-int-) | 表示工作表类型。 |
| [setUniqueId(String value)](#setUniqueId-java.lang.String-) | 设置唯一标识符，它与 \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\} 相同。 |
| [setViewType(int value)](#setViewType-int-) | 设置视图类型。 |
| [setVisibilityType(int value)](#setVisibilityType-int-) | 指示此工作表的可见状态。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 表示工作表是否可见。 |
| [setVisible(boolean isVisible, boolean ignoreError)](#setVisible-boolean-boolean-) | 设置可见选项。 |
| [setZoom(int value)](#setZoom-int-) | 表示以百分比计的缩放因子。 |
| [split()](#split--) | 拆分窗口。 |
| [startAccessCache(int opts)](#startAccessCache-int-) | 启动使用缓存访问此工作表数据的会话。 |
| [toString()](#toString--) | 返回表示当前 Worksheet 对象的字符串。 |
| [unFreezePanes()](#unFreezePanes--) | 取消冻结工作表中的窗格。 |
| [unprotect()](#unprotect--) | 取消保护工作表。 |
| [unprotect(String password)](#unprotect-java.lang.String-) | 取消保护工作表。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [xmlMapQuery(String path, XmlMap xmlMap)](#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | 查询映射/链接到特定 XML 映射路径的单元格区域。 |
### addPageBreaks(String cellName) {#addPageBreaks-java.lang.String-}
```
public void addPageBreaks(String cellName)
```


添加分页符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String |  |

### advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly) {#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public void advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)
```


使用复杂条件过滤数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isFilter | boolean | 指示是否在原位过滤列表。 |
| listRange | java.lang.String | 列表范围。 |
| criteriaRange | java.lang.String | 条件范围。 |
| copyTo | java.lang.String | 复制数据的目标范围。 |
| uniqueRecordOnly | boolean | 仅显示或复制唯一的行。 |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


自动调整列宽。

**Remarks**

AutoFitColumn is an imprecise function.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


自动调整列宽。

**Remarks**

此方法根据行内单元格范围的内容自动调整行的大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |
| firstRow | int | 第一行索引。 |
| lastRow | int | 最后一行索引。 |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```


自动调整此工作表中所有列的宽度。

### autoFitColumns(AutoFitterOptions options) {#autoFitColumns-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(AutoFitterOptions options)
```


自动调整此工作表中所有列的宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | 自动适配选项 |

### autoFitColumns(int firstColumn, int lastColumn) {#autoFitColumns-int-int-}
```
public void autoFitColumns(int firstColumn, int lastColumn)
```


自动调整列的宽度。

**Remarks**

AutoFitColumn is an imprecise function.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstColumn | int | 第一列索引。 |
| lastColumn | int | 最后一列索引。 |

### autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```


自动调整列的宽度。

**Remarks**

AutoFitColumn is an imprecise function.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstColumn | int | 第一列索引。 |
| lastColumn | int | 最后一列索引。 |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | 自动适配选项 |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn) {#autoFitColumns-int-int-int-int-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```


自动调整列的宽度。

**Remarks**

AutoFitColumn is an imprecise function.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 第一行索引。 |
| firstColumn | int | 第一列索引。 |
| lastRow | int | 最后一行索引。 |
| lastColumn | int | 最后一列索引。 |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)
```


自动调整列的宽度。

**Remarks**

AutoFitColumn is an imprecise function.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 第一行索引。 |
| firstColumn | int | 第一列索引。 |
| lastRow | int | 最后一行索引。 |
| lastColumn | int | 最后一列索引。 |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | 自动适配选项 |

### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


自动调整行高。

**Remarks**

AutoFitRow is an imprecise function.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


自动调整行高。

**Remarks**

此方法根据行内单元格范围的内容自动调整行的大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |
| firstColumn | int | 第一列索引。 |
| lastColumn | int | 最后一列索引。 |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```


自动调整行高。

**Remarks**

此方法根据行内单元格范围的内容自动调整行的大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |
| firstColumn | int | 第一列索引。 |
| lastColumn | int | 最后一列索引。 |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | 自动适配器选项 |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


在矩形范围内自动调整行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| endRow | int | 结束行索引。 |
| startColumn | int | 起始列索引。 |
| endColumn | int | 结束列索引。 |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


自动调整此工作表中所有行的高度。

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


自动调整此工作表中所有行的高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| onlyAuto | boolean | True，仅在行高未自定义时自动适配行高。 |

### autoFitRows(AutoFitterOptions options) {#autoFitRows-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(AutoFitterOptions options)
```


自动调整此工作表中所有行的高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | 自动适配器选项 |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


在范围内自动调整行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| endRow | int | 结束行索引。 |

### autoFitRows(int startRow, int endRow, AutoFitterOptions options) {#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(int startRow, int endRow, AutoFitterOptions options)
```


在范围内自动调整行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| endRow | int | 结束行索引。 |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | 自动适配器的选项。 |

### calculateArrayFormula(String formula, CalculationOptions opts) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts)
```


将公式计算为数组公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 待计算的公式。 |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | 计算公式的选项 |

**Returns:**
java.lang.Object[][]
### calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)
```


将公式计算为数组公式。

**Remarks**

该公式将被视为动态数组公式，用于计算维度和结果。用户指定的最大维度用于计算结果为大型数据集的情况（例如，计算结果可能对应整行或整列数据），但根据业务需求或性能考虑，用户并不需要如此大的数组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 待计算的公式。 |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | 计算公式的选项 |
| maxRowCount | int | 结果数据的最大行数。如果为非正数或大于实际行数，则使用实际行数。 |
| maxColumnCount | int | 结果数据的最大列数。如果为非正数或大于实际列数，则使用实际列数。 |

**Returns:**
java.lang.Object[][] - 计算后的公式结果。
### calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData) {#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-}
```
public Object[][] calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)
```


将公式计算为数组公式。

**Remarks**

该公式将被视为动态数组公式，用于计算维度和结果。用户指定的最大维度用于计算结果为大型数据集的情况（例如，计算结果可能对应整行或整列数据），但根据业务需求或性能考虑，用户并不需要如此大的数组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 待计算的公式。 |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项 |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | 计算公式的选项 |
| baseCellRow | int | 基准单元格的行索引。 |
| baseCellColumn | int | 基准单元格的列索引。 |
| maxRowCount | int | 结果数据的最大行数。如果为非正数或大于实际行数，则使用实际行数。 |
| maxColumnCount | int | 结果数据的最大列数。如果为非正数或大于实际列数，则使用实际列数。 |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | 计算数据。它用于用户在实现自定义计算引擎时需要计算一些静态公式的情况。对于此类情况，用户需要使用提供给 [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) 的计算数据进行指定。 |

**Returns:**
java.lang.Object[][] - 计算后的公式结果。
### calculateFormula(CalculationOptions options, boolean recursive) {#calculateFormula-com.aspose.cells.CalculationOptions-boolean-}
```
public void calculateFormula(CalculationOptions options, boolean recursive)
```


计算此工作表中的所有公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | 计算的选项 |
| recursive | boolean | True 表示如果工作表的单元格依赖于其他工作表的单元格，则其他工作表中的依赖单元格也会被计算。False 表示工作表中的所有公式已被计算，且数值是正确的。 |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


计算一个公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 待计算的公式。 |

**Returns:**
java.lang.Object - 计算后的公式结果。
### calculateFormula(String formula, CalculationOptions opts) {#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object calculateFormula(String formula, CalculationOptions opts)
```


直接计算公式表达式。

**Remarks**

该公式将像设置在单元格 A1 中一样被计算，并且将被视为普通公式。如果需要将公式作为数组公式计算并获取计算结果的数组，请改用 [calculateArrayFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-CalculationOptions-)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 待计算的公式。 |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | 计算公式的选项 |

**Returns:**
java.lang.Object - 给定公式的计算结果。返回的对象可能是 [Cell.getValue()](../../com.aspose.cells/cell\#getValue--) 的可能类型之一，或 ReferredArea。
### calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData) {#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-}
```
public Object calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)
```


直接计算公式表达式。

**Remarks**

该公式将像设置在指定基准单元格一样被计算，并且将被视为普通公式。如果需要将公式作为数组公式计算并获取计算结果的数组，请改用 [calculateArrayFormula(String,FormulaParseOptions,CalculationOptions,int,int,int,int,CalculationData)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-FormulaParseOptions-CalculationOptions-int-int-int-int-CalculationData-)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 待计算的公式。 |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | 解析公式的选项。 |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | 计算公式的选项。 |
| baseCellRow | int | 基准单元格的行索引。 |
| baseCellColumn | int | 基准单元格的列索引。 |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | 计算数据。它用于用户在实现自定义计算引擎时需要计算一些静态公式的情况。对于此类情况，用户需要使用提供给 [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) 的计算数据进行指定。 |

**Returns:**
java.lang.Object - 给定公式的计算结果。返回的对象可能是 [Cell.getValue()](../../com.aspose.cells/cell\#getValue--) 的可能类型之一，或 ReferredArea。
### clearComments() {#clearComments--}
```
public void clearComments()
```


清除设计器电子表格中的所有批注。

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


关闭使用缓存访问此工作表数据的会话。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). 数据访问的选项 |

### convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn) {#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-}
```
public String convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)
```


转换公式引用样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 待转换的公式。 |
| toR1C1 | boolean | 将公式转换为何种引用样式。如果原始公式使用 A1 引用样式，则此值应为 true，以便公式从 A1 转换为 R1C1 引用样式；如果原始公式使用 R1C1 引用样式，则此值应为 false，以便公式从 R1C1 转换为 A1 引用样式； |
| baseCellRow | int | 基准单元格的行索引。 |
| baseCellColumn | int | 基准单元格的列索引。 |

**Returns:**
java.lang.String - 转换后的公式。
### copy(Worksheet sourceSheet) {#copy-com.aspose.cells.Worksheet-}
```
public void copy(Worksheet sourceSheet)
```


复制来自另一个工作表的内容和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | 源工作表。 |

### copy(Worksheet sourceSheet, CopyOptions copyOptions) {#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-}
```
public void copy(Worksheet sourceSheet, CopyOptions copyOptions)
```


复制来自另一个工作表的内容和格式。

**Remarks**

您可以从同一文件或其他文件中的另一个工作表复制数据。但此方法不支持复制绘图对象，例如批注、图像和图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | 源工作表。 |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

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
### filter(CellArea ca) {#filter-com.aspose.cells.CellArea-}
```
public void filter(CellArea ca)
```


筛选该范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 范围 |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


在工作表中指定的单元格处冻结窗格。

**Remarks**

行索引和列索引不能全部为零。行数和列数也不能全部为零。

前两个参数指定冻结位置，后两个参数指定左上窗格中冻结的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |
| freezedRows | int | 顶部窗格中可见行数，不超过行索引。 |
| freezedColumns | int | 左侧窗格中可见列数，不超过列索引。 |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


在工作表中指定的单元格处冻结窗格。

**Remarks**

行索引和列索引不能全部为零。行数和列数也不能全部为零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |
| freezedRows | int | 顶部窗格中可见行数，不超过行索引。 |
| freezedColumns | int | 左侧窗格中可见列数，不超过列索引。 |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


获取工作表中的活动单元格。

**Returns:**
java.lang.String
### getAdvancedFilter() {#getAdvancedFilter--}
```
public AdvancedFilter getAdvancedFilter()
```


获取高级筛选的设置。

**Returns:**
[AdvancedFilter](../../com.aspose.cells/advancedfilter) - 
### getAllPictures() {#getAllPictures--}
```
public Picture[] getAllPictures()
```


获取所有图片，包括嵌入单元格以及位于单元格上方的图像。

**Returns:**
com.aspose.cells.Picture[] -
### getAllowEditRanges() {#getAllowEditRanges--}
```
public ProtectedRangeCollection getAllowEditRanges()
```


获取工作表中允许编辑范围的集合。

**Returns:**
[ProtectedRangeCollection](../../com.aspose.cells/protectedrangecollection)
### getAreasOfXmlMapQuery(String path, XmlMap xmlMap) {#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public CellArea[] getAreasOfXmlMapQuery(String path, XmlMap xmlMap)
```


查询映射/链接到特定 XML 映射路径的单元格区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | java.lang.String | XML 元素路径 |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | 如果要查询特定映射中的特定路径，请指定 XML 映射 |

**Returns:**
com.aspose.cells.CellArea[] - [CellArea](../../com.aspose.cells/cellarea) 列表，映射/链接到 XML 映射的特定路径，如果没有任何映射/链接，则返回空列表。
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


表示指定工作表的自动筛选。

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


获取工作表的背景图像。

**Returns:**
byte[]
### getCellWatches() {#getCellWatches--}
```
public CellWatchCollection getCellWatches()
```


获取此工作表在“监视窗口”中被监视的单元格集合。

**Returns:**
[CellWatchCollection](../../com.aspose.cells/cellwatchcollection)
### getCells() {#getCells--}
```
public Cells getCells()
```


获取 [Cells](../../com.aspose.cells/cells) 集合。

**Returns:**
[Cells](../../com.aspose.cells/cells)
### getCharts() {#getCharts--}
```
public ChartCollection getCharts()
```


获取 [Chart](../../com.aspose.cells/chart) 集合

**Returns:**
[ChartCollection](../../com.aspose.cells/chartcollection)
### getCheckBoxes() {#getCheckBoxes--}
```
public CheckBoxCollection getCheckBoxes()
```


获取 [CheckBox](../../com.aspose.cells/checkbox) 集合。

**Returns:**
[CheckBoxCollection](../../com.aspose.cells/checkboxcollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


获取工作表代码名称。

**Returns:**
java.lang.String
### getComments() {#getComments--}
```
public CommentCollection getComments()
```


获取 [Comment](../../com.aspose.cells/comment) 集合。

**Returns:**
[CommentCollection](../../com.aspose.cells/commentcollection)
### getConditionalFormattings() {#getConditionalFormattings--}
```
public ConditionalFormattingCollection getConditionalFormattings()
```


获取工作表中的 ConditionalFormattings。

**Returns:**
[ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection)
### getCustomProperties() {#getCustomProperties--}
```
public CustomPropertyCollection getCustomProperties()
```


获取表示与工作表关联的标识信息的对象。

**Remarks**

Worksheet.CustomProperties 提供了一种首选机制来存储任意数据。它支持传统的第三方文档组件，以及对二进制部分有严格需求的情况。

**Returns:**
[CustomPropertyCollection](../../com.aspose.cells/custompropertycollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


指示指定的工作表是否从右向左显示，而不是从左向右。默认值为 false。

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


如果显示零值，则为 True。

**Returns:**
boolean
### getErrorCheckOptions() {#getErrorCheckOptions--}
```
public ErrorCheckOptionCollection getErrorCheckOptions()
```


获取在特定范围上应用的错误检查设置。

**Returns:**
[ErrorCheckOptionCollection](../../com.aspose.cells/errorcheckoptioncollection)
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


表示第一个可见列的索引。

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


表示第一个可见行的索引。

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


获取冻结窗格。

**Returns:**
int[] - 返回 null 表示工作表未冻结 0:行索引;1:列;2:冻结行;3:冻结行
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


获取网格线的颜色

**Returns:**
[Color](../../com.aspose.cells/color)
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public HorizontalPageBreakCollection getHorizontalPageBreaks()
```


获取 [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection) 集合。

**Returns:**
[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)
### getHyperlinks() {#getHyperlinks--}
```
public HyperlinkCollection getHyperlinks()
```


获取 [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection) 集合。

**Returns:**
[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


获取工作表集合中工作表的索引。

**Returns:**
int
### getListObjects() {#getListObjects--}
```
public ListObjectCollection getListObjects()
```


获取此工作表中的所有 ListObjects。

**Returns:**
[ListObjectCollection](../../com.aspose.cells/listobjectcollection)
### getName() {#getName--}
```
public String getName()
```


获取工作表的名称。

**Remarks**

工作表名称的最大长度为 31。且不能为两个工作表分配相同的名称（不区分大小写）。例如，您不能将 "SheetName1" 设置为第一个工作表，同时将 "SHEETNAME1" 设置为第二个工作表。

**Returns:**
java.lang.String
### getOleObjects() {#getOleObjects--}
```
public OleObjectCollection getOleObjects()
```


表示工作表中 [OleObject](../../com.aspose.cells/oleobject) 的集合。

**Returns:**
[OleObjectCollection](../../com.aspose.cells/oleobjectcollection)
### getOutline() {#getOutline--}
```
public Outline getOutline()
```


获取此工作表上的大纲。

**Returns:**
[Outline](../../com.aspose.cells/outline)
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


表示此工作表中的页面设置描述。

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPaneState() {#getPaneState--}
```
public int getPaneState()
```


指示窗格是否具有水平或垂直拆分，以及这些拆分是否已冻结。

参见 [PaneStateType](../../com.aspose.cells/panestatetype)。

**Returns:**
int
### getPanes() {#getPanes--}
```
public PaneCollection getPanes()
```


获取窗口窗格。

**Remarks**

如果窗口未被拆分或冻结。

**Returns:**
[PaneCollection](../../com.aspose.cells/panecollection)
### getPictures() {#getPictures--}
```
public PictureCollection getPictures()
```


获取 [Picture](../../com.aspose.cells/picture) 集合。

**Returns:**
[PictureCollection](../../com.aspose.cells/picturecollection)
### getPivotTables() {#getPivotTables--}
```
public PivotTableCollection getPivotTables()
```


获取此工作表中的所有数据透视表。

**Returns:**
[PivotTableCollection](../../com.aspose.cells/pivottablecollection)
### getPrintingPageBreaks(ImageOrPrintOptions options) {#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-}
```
public CellArea[] getPrintingPageBreaks(ImageOrPrintOptions options)
```


获取自动分页符。

**Remarks**

每个单元格区域代表一张纸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | 打印选项 |

**Returns:**
com.aspose.cells.CellArea[] - 自动分页区域。
### getProtection() {#getProtection--}
```
public Protection getProtection()
```


表示工作表可用的各种保护选项类型。支持 ExcelXP 及以上版本的高级保护选项。

**Remarks**

此属性可以在所有版本的 Excel 文件中保护工作表，并支持 ExcelXP 及以上版本的高级保护选项。

**Returns:**
[Protection](../../com.aspose.cells/protection)
### getQueryTables() {#getQueryTables--}
```
public QueryTableCollection getQueryTables()
```


获取工作表中的 [QueryTableCollection](../../com.aspose.cells/querytablecollection)。

**Returns:**
[QueryTableCollection](../../com.aspose.cells/querytablecollection)
### getScenarios() {#getScenarios--}
```
public ScenarioCollection getScenarios()
```


获取 [Scenario](../../com.aspose.cells/scenario) 的集合。

**Returns:**
[ScenarioCollection](../../com.aspose.cells/scenariocollection)
### getSelectedAreas() {#getSelectedAreas--}
```
public Range[] getSelectedAreas()
```


获取设计器电子表格中选定的单元格范围。

**Returns:**
com.aspose.cells.Range[] - 返回所有选定的范围。
### getSelectedRanges() {#getSelectedRanges--}
```
public ArrayList getSelectedRanges()
```


获取设计器电子表格中选定的单元格范围。

**Remarks**

NOTE: 此方法现已过时。相反，请使用 Worksheet.GetSelectedAreas() 方法。此属性将在自 2025 年 3 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.util.ArrayList - 包含所选范围的 ArrayList。
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


返回此工作表中的所有绘图形状。

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTypeIcons() {#getShowDataTypeIcons--}
```
public boolean getShowDataTypeIcons()
```


指示是否显示数据类型图标。

**Returns:**
boolean
### getShowFormulas() {#getShowFormulas--}
```
public boolean getShowFormulas()
```


指示是否显示公式或其结果。

**Returns:**
boolean
### getSlicers() {#getSlicers--}
```
public SlicerCollection getSlicers()
```


获取工作表中的 Slicer 集合

**Returns:**
[SlicerCollection](../../com.aspose.cells/slicercollection)
### getSmartTagSetting() {#getSmartTagSetting--}
```
public SmartTagSetting getSmartTagSetting()
```


获取工作表的所有 [SmartTagCollection](../../com.aspose.cells/smarttagcollection) 对象。

**Returns:**
[SmartTagSetting](../../com.aspose.cells/smarttagsetting)
### getSparklineGroups() {#getSparklineGroups--}
```
public SparklineGroupCollection getSparklineGroups()
```


获取工作表中的 sparkline 组。

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


表示工作表选项卡颜色。

**Remarks**

此功能仅在 ExcelXP（Excel2002）及更高版本中受支持。如果将文件另存为 Excel97 或 Excel2000 格式，则会被省略。

**Returns:**
[Color](../../com.aspose.cells/color)
### getTabId() {#getTabId--}
```
public int getTabId()
```


指定工作表的内部标识符。

**Returns:**
int
### getTextBoxes() {#getTextBoxes--}
```
public TextBoxCollection getTextBoxes()
```


获取一个 [TextBox](../../com.aspose.cells/textbox) 集合。

**Returns:**
[TextBoxCollection](../../com.aspose.cells/textboxcollection)
### getTimelines() {#getTimelines--}
```
public TimelineCollection getTimelines()
```


获取工作表中的 Timeline 集合

**Returns:**
[TimelineCollection](../../com.aspose.cells/timelinecollection)
### getTransitionEntry() {#getTransitionEntry--}
```
public boolean getTransitionEntry()
```


指示是否启用了 Transition Formula Entry（Lotus 兼容）选项。

**Returns:**
boolean
### getTransitionEvaluation() {#getTransitionEvaluation--}
```
public boolean getTransitionEvaluation()
```


指示是否启用了 Transition Formula Evaluation（Lotus 兼容）选项。

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


表示工作表类型。

请参阅 [SheetType](../../com.aspose.cells/sheettype)。

**Returns:**
int
### getUniqueId() {#getUniqueId--}
```
public String getUniqueId()
```


获取唯一 ID，它与 \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\} 相同。

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public ValidationCollection getValidations()
```


获取工作表中的数据验证设置集合。

**Returns:**
[ValidationCollection](../../com.aspose.cells/validationcollection)
### getVerticalPageBreaks() {#getVerticalPageBreaks--}
```
public VerticalPageBreakCollection getVerticalPageBreaks()
```


获取 [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection) 集合。

**Returns:**
[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)
### getViewType() {#getViewType--}
```
public int getViewType()
```


获取视图类型。

请参阅 [ViewType](../../com.aspose.cells/viewtype)。

**Returns:**
int
### getVisibilityType() {#getVisibilityType--}
```
public int getVisibilityType()
```


指示此工作表的可见状态。

请参阅 [VisibilityType](../../com.aspose.cells/visibilitytype)。

**Returns:**
int
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


获取包含此工作表的工作簿对象。

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


表示百分比的缩放因子。应在 10 到 400 之间。

**Remarks**

请先设置视图类型。

**Returns:**
int
### hasAutofilter() {#hasAutofilter--}
```
public boolean hasAutofilter()
```


指示此工作表是否具有自动筛选。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


获取一个值，指示网格线是否可见。默认值为 true。

**Returns:**
boolean
### isOutlineShown() {#isOutlineShown--}
```
public boolean isOutlineShown()
```


指示是否显示大纲。

**Returns:**
boolean
### isPageBreakPreview() {#isPageBreakPreview--}
```
public boolean isPageBreakPreview()
```


指示指定的工作表是以普通视图还是分页预览方式显示。

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


指示工作表是否受保护。

**Returns:**
boolean
### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}
```
public boolean isRowColumnHeadersVisible()
```


获取一个值，指示工作表是否显示行和列标题。默认值为 true。

**Returns:**
boolean
### isRulerVisible() {#isRulerVisible--}
```
public boolean isRulerVisible()
```


指示标尺是否可见。此属性仅在分页预览时适用。

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


指示打开工作簿时是否选中此工作表。

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


表示工作表是否可见。

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


将工作表移动到电子表格中的其他位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 目标工作表索引。 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### protect(int type) {#protect-int-}
```
public void protect(int type)
```


保护工作表。

**Remarks**

此方法在不使用密码的情况下保护工作表。它可以在所有版本的 Excel 文件中保护工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). 保护类型。 |

### protect(int type, String password, String oldPassword) {#protect-int-java.lang.String-java.lang.String-}
```
public void protect(int type, String password, String oldPassword)
```


保护工作表。

**Remarks**

此方法可以在所有版本的 Excel 文件中保护工作表。

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = excel.getWorksheets().get(0);
         //Protecting the worksheet with a password
         worksheet.protect(ProtectionType.ALL, "aspose", null);
         //Saving the modified Excel file in default (that is Excel 20003) format
         excel.save("output.xls");
         //Closing the file stream to free all resources
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). 保护类型。 |
| 密码 | java.lang.String | 密码。 |
| oldPassword | java.lang.String | 如果工作表已被密码保护，请提供旧密码。否则，您可以将此参数设置为 null 值或空字符串。 |

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


刷新此工作表中的所有数据透视表。

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


刷新此工作表中的所有数据透视表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | 用于刷新数据透视表数据源的选项。 |

**Returns:**
boolean
### removeAllDrawingObjects() {#removeAllDrawingObjects--}
```
public void removeAllDrawingObjects()
```


删除此工作表中的所有绘图对象。

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


移除工作表的自动筛选。

### removeSplit() {#removeSplit--}
```
public void removeSplit()
```


移除拆分窗口。

### replace(String oldString, String newString) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String oldString, String newString)
```


将所有单元格的文本替换为新字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldString | java.lang.String | 旧字符串值。 |
| newString | java.lang.String | 新字符串值。 |

**Returns:**
int
### selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers) {#selectRange-int-int-int-int-boolean-}
```
public void selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)
```


选择一个范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行。 |
| startColumn | int | 起始列 |
| totalRows | int | 行数。 |
| totalColumns | int | 列数 |
| removeOthers | boolean | True 表示删除其他已选择的范围，仅选择此范围。 |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


设置工作表中的活动单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


设置工作表的背景图像。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setCodeName(String value) {#setCodeName-java.lang.String-}
```
public void setCodeName(String value)
```


获取工作表代码名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


指示指定的工作表是否从右向左显示，而不是从左向右。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


如果显示零值，则为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


表示第一个可见列的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


表示第一个可见行的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


设置网格线的颜色

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


设置一个值，指示网格线是否可见。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置工作表的名称。

**Remarks**

工作表名称的最大长度为 31。且不能为两个工作表分配相同的名称（不区分大小写）。例如，您不能将 "SheetName1" 设置为第一个工作表，同时将 "SHEETNAME1" 设置为第二个工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


指示是否显示大纲。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPageBreakPreview(boolean value) {#setPageBreakPreview-boolean-}
```
public void setPageBreakPreview(boolean value)
```


指示指定的工作表是以普通视图还是分页预览方式显示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRowColumnHeadersVisible(boolean value) {#setRowColumnHeadersVisible-boolean-}
```
public void setRowColumnHeadersVisible(boolean value)
```


设置一个值，指示工作表是否显示行和列标题。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRulerVisible(boolean value) {#setRulerVisible-boolean-}
```
public void setRulerVisible(boolean value)
```


指示标尺是否可见。此属性仅在分页预览时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


指示打开工作簿时是否选中此工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowDataTypeIcons(boolean value) {#setShowDataTypeIcons-boolean-}
```
public void setShowDataTypeIcons(boolean value)
```


指示是否显示数据类型图标。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowFormulas(boolean value) {#setShowFormulas-boolean-}
```
public void setShowFormulas(boolean value)
```


指示是否显示公式或其结果。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.cells.Color-}
```
public void setTabColor(Color value)
```


表示工作表选项卡颜色。

**Remarks**

此功能仅在 ExcelXP（Excel2002）及更高版本中受支持。如果将文件另存为 Excel97 或 Excel2000 格式，则会被省略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setTabId(int value) {#setTabId-int-}
```
public void setTabId(int value)
```


指定工作表的内部标识符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTransitionEntry(boolean value) {#setTransitionEntry-boolean-}
```
public void setTransitionEntry(boolean value)
```


指示是否启用了 Transition Formula Entry（Lotus 兼容）选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTransitionEvaluation(boolean value) {#setTransitionEvaluation-boolean-}
```
public void setTransitionEvaluation(boolean value)
```


指示是否启用了 Transition Formula Evaluation（Lotus 兼容）选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


表示工作表类型。

请参阅 [SheetType](../../com.aspose.cells/sheettype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setUniqueId(String value) {#setUniqueId-java.lang.String-}
```
public void setUniqueId(String value)
```


设置唯一标识符，它与 \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\} 相同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setViewType(int value) {#setViewType-int-}
```
public void setViewType(int value)
```


设置视图类型。

请参阅 [ViewType](../../com.aspose.cells/viewtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setVisibilityType(int value) {#setVisibilityType-int-}
```
public void setVisibilityType(int value)
```


指示此工作表的可见状态。

请参阅 [VisibilityType](../../com.aspose.cells/visibilitytype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


表示工作表是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setVisible(boolean isVisible, boolean ignoreError) {#setVisible-boolean-boolean-}
```
public void setVisible(boolean isVisible, boolean ignoreError)
```


设置可见选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isVisible | boolean | 工作表是否可见 |
| ignoreError | boolean | 如果此选项无效，是否忽略错误。 |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


表示百分比的缩放因子。应在 10 到 400 之间。

**Remarks**

请先设置视图类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### split() {#split--}
```
public void split()
```


拆分窗口。

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


启动使用缓存访问此工作表数据的会话。

**Remarks**

完成数据访问后，应使用相同的选项调用 [closeAccessCache(int)](../../com.aspose.cells/worksheet\#closeAccessCache-int-)，以清除所有缓存并恢复正常访问模式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). 数据访问的选项 |

### toString() {#toString--}
```
public String toString()
```


返回表示当前 Worksheet 对象的字符串。

**Returns:**
java.lang.String -
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


取消冻结工作表中的窗格。

### unprotect() {#unprotect--}
```
public void unprotect()
```


取消保护工作表。

**Remarks**

此方法取消对未设置密码的工作表的保护。

### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


取消保护工作表。

**Remarks**

如果工作表未设置密码进行保护，您可以将 password 参数设为 null 值或空字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 密码 | java.lang.String | 密码 |

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

### xmlMapQuery(String path, XmlMap xmlMap) {#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public ArrayList xmlMapQuery(String path, XmlMap xmlMap)
```


查询映射/链接到特定 XML 映射路径的单元格区域。

**Remarks**

注意：此方法现已过时。请改用 Worksheet.GetAreasOfXmlMapQuery() 方法。此属性将在自 2026 年 8 月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | java.lang.String | XML 元素路径 |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | 如果要查询特定映射中的特定路径，请指定 XML 映射 |

**Returns:**
java.util.ArrayList - 与特定 XML 映射路径映射/链接的 [CellArea](../../com.aspose.cells/cellarea) 列表，如果没有任何映射/链接，则返回空列表。
