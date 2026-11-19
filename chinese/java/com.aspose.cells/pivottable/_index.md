---
title: "数据透视表"
second_title: "Aspose.Cells for Java API 参考"
description: "PivotTable 的摘要描述。"
type: docs
url: /zh/java/com.aspose.cells/pivottable/
---

**Inheritance:**
java.lang.Object
```
public class PivotTable
```

PivotTable 的摘要描述。

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
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
          PivotTableCalculateOption calculateOption = new PivotTableCalculateOption();
          calculateOption.setRefreshData(true);
          calculateOption.setRefreshCharts(true);
          pivot.calculateData(calculateOption); 
 
         //do your business
 
         book.save("out.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addCalculatedField(String name, String formula)](#addCalculatedField-java.lang.String-java.lang.String-) | 向数据透视字段添加计算字段并将其拖动到数据区域。 |
| [addCalculatedField(String name, String formula, boolean dragToDataArea)](#addCalculatedField-java.lang.String-java.lang.String-boolean-) | 向数据透视字段添加计算字段。 |
| [addFieldToArea(int fieldType, PivotField pivotField)](#addFieldToArea-int-com.aspose.cells.PivotField-) | 将字段添加到特定区域。 |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | 将字段添加到特定区域。 |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | 将字段添加到特定区域。 |
| [calculateData()](#calculateData--) | 将数据透视表的数据计算到单元格。 |
| [calculateData(PivotTableCalculateOption option)](#calculateData-com.aspose.cells.PivotTableCalculateOption-) | 使用选项计算数据透视表。 |
| [calculateRange()](#calculateRange--) | 计算数据透视表的范围。 |
| [changeDataSource(String[] source)](#changeDataSource-java.lang.String---) | 更改数据透视表的数据源。 |
| [clearAll()](#clearAll--) | 从区域中移除所有字段。 |
| [clearData()](#clearData--) | 清除 PivotTable 视图的数据和格式。 |
| [clearFilters()](#clearFilters--) | 清除此数据透视表的所有筛选。 |
| [copyStyle(PivotTable pivotTable)](#copyStyle-com.aspose.cells.PivotTable-) | 从另一个数据透视表复制命名样式。 |
| [dispose()](#dispose--) | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportViewToJson(PivotViewToJsonOptions options)](#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-) | 将数据透视视图导出为 JSON。 |
| [fields(int fieldType)](#fields-int-) | 根据字段类型获取特定字段。 |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | 格式化数据透视表的选定区域。 |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | 格式化数据透视表的选定区域。 |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | 格式化数据透视表区域中的单元格 |
| [formatAll(Style style)](#formatAll-com.aspose.cells.Style-) | 格式化数据透视表区域中的所有单元格 |
| [formatRow(int row, Style style)](#formatRow-int-com.aspose.cells.Style-) | 格式化数据透视表区域中的行数据 |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--) | 指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。 |
| [getAltTextDescription()](#getAltTextDescription--) | 获取替代文本的描述。 |
| [getAltTextTitle()](#getAltTextTitle--) | 获取替代文本的标题。 |
| [getAutoFormatType()](#getAutoFormatType--) | 获取数据透视表的自动格式类型。 |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--) | 指示在更新时是否自动适应列宽 |
| [getBaseFields()](#getBaseFields--) | 返回数据透视表中的所有基础数据透视字段。 |
| [getButtonArea(int axisType)](#getButtonArea-int-) | 获取包含字段按钮的区域。 |
| [getCellByDisplayName(String displayName)](#getCellByDisplayName-java.lang.String-) | 通过 PivotField 的显示名称获取 [Cell](../../com.aspose.cells/cell) 对象。 |
| [getChildren()](#getChildren--) | 获取使用此数据透视表数据作为数据源的子数据透视表。 |
| [getClass()](#getClass--) |  |
| [getColumnFields()](#getColumnFields--) | 返回当前显示为列字段的 PivotFields 对象。 |
| [getColumnGrand()](#getColumnGrand--) | 指示数据透视表报告是否显示列的总计。 |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--) | 获取数据透视表列标题的自定义标题。 |
| [getColumnRange()](#getColumnRange--) | 返回一个 CellArea 对象，表示包含数据透视表报告中列区域的范围。 |
| [getConditionalFormats()](#getConditionalFormats--) | 获取数据透视表的条件格式。 |
| [getCustomListSort()](#getCustomListSort--) | 指示在排序数据时是否考虑内置自定义列表 |
| [getDataBodyRange()](#getDataBodyRange--) | 返回一个 [CellArea](../../com.aspose.cells/cellarea) 对象，表示在标题行和插入行之间的列表中包含数据区域的范围。 |
| [getDataField()](#getDataField--) | 获取一个 [PivotField](../../com.aspose.cells/pivotfield) 对象，表示数据透视表中的所有数据字段。 |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--) | 获取 PivotTable 中值区域字段标题的名称。 |
| [getDataFields()](#getDataFields--) | 获取一个 [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)，它表示 PivotTable 中的所有数据字段。 |
| [getDataSource()](#getDataSource--) | 获取 PivotTable 的数据源。 |
| [getDependentPivotTables()](#getDependentPivotTables--) | 获取所有使用此 PivotTable 作为数据源的 [PivotTable](../../com.aspose.cells/pivottable)s。 |
| [getDisplayErrorString()](#getDisplayErrorString--) | 指示 PivotTable 报表是否在包含错误的单元格中显示自定义字符串。 |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--) | 指示当 PivotTable 的数据区域为空时，行和列区域中的项目是否可见。 |
| [getDisplayNullString()](#getDisplayNullString--) | 指示 PivotTable 报表在值为 null 时是否显示自定义字符串。 |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--) | 指定一个布尔值，指示是否允许用户编辑 pivottable 数据区域中的单元格。 |
| [getEnableDrilldown()](#getEnableDrilldown--) | 指示是否启用下钻。 |
| [getEnableFieldDialog()](#getEnableFieldDialog--) | 指示当用户双击 PivotTable 字段时，PivotTable 字段对话框是否可用。 |
| [getEnableFieldList()](#getEnableFieldList--) | 指示在 Excel 视图中是否可用 PivotTable 的字段列表。 |
| [getEnableWizard()](#getEnableWizard--) | 指示 PivotTable 向导是否可用。 |
| [getErrorString()](#getErrorString--) | 获取在 DisplayErrorString 属性为 true 时显示在包含错误的单元格中的字符串。默认值为空字符串。 |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--) | 获取外部连接数据源。 |
| [getFieldListSortAscending()](#getFieldListSortAscending--) | 指示 PivotTable 中的字段在字段列表中是否以非默认顺序排序。 |
| [getFields(int fieldType)](#getFields-int-) | 按区域获取特定的 pivot field 列表。 |
| [getFilterArea()](#getFilterArea--) | 获取筛选区域的范围。 |
| [getGrandTotalName()](#getGrandTotalName--) | 返回显示在总计列或行标题中的标签。 |
| [getHorizontalBreaks()](#getHorizontalBreaks--) | 获取 PivotTable 水平分页符的行索引列表。 |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | 获取此 PivotTable 的水平分页符。 |
| [getIndent()](#getIndent--) | 指定紧凑轴的缩进增量，可用于将 Report Layout 设置为紧凑形式。 |
| [getItemPrintTitles()](#getItemPrintTitles--) | 指示是否应在每页打印的顶部重复 PivotItem 名称。 |
| [getManualUpdate()](#getManualUpdate--) | 指示 PivotTable 报表是否仅在用户请求时重新计算。 |
| [getMergeLabels()](#getMergeLabels--) | 获取是否合并跨多个单元格的行/列字段标签。 |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | 指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。 |
| [getName()](#getName--) | 获取 PivotTable 的名称 |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--) | 获取外部源数据连接的名称。 |
| [getNullString()](#getNullString--) | 获取在 DisplayNullString 属性为 true 时显示在包含 null 值的单元格中的字符串。默认值为空字符串。 |
| [getPageFieldOrder()](#getPageFieldOrder--) | 获取页面字段添加到数据透视表报告布局中的顺序。 |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--) | 获取数据透视表报告中每列或每行的页面字段数量。 |
| [getPageFields()](#getPageFields--) | 返回当前显示为页面字段的 [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)。 |
| [getPivotCache()](#getPivotCache--) | 获取数据源。 |
| [getPivotFilters()](#getPivotFilters--) | 返回数据透视表中的所有筛选器。 |
| [getPivotFormatConditions()](#getPivotFormatConditions--) | 获取数据透视表的格式条件。 |
| [getPivotFormats()](#getPivotFormats--) | 获取应用于此数据透视表的所有单元格格式。 |
| [getPivotTableStyle()](#getPivotTableStyle--) | 获取此数据透视表的 [TableStyle](../../com.aspose.cells/tablestyle) 设置。 |
| [getPivotTableStyleName()](#getPivotTableStyleName--) | 获取数据透视表的样式名称。 |
| [getPivotTableStyleType()](#getPivotTableStyleType--) | 获取内置的数据透视表样式。 |
| [getPivotTablesWithSamePivotCache()](#getPivotTablesWithSamePivotCache--) | 获取具有相同数据透视缓存的所有数据透视表。 |
| [getPreserveCellFormattingOnUpdate()](#getPreserveCellFormattingOnUpdate--) | 指示在刷新或重新计算数据透视表时是否保留单元格格式 ([PivotTableFormat](../../com.aspose.cells/pivottableformat))。 |
| [getPreserveFormatting()](#getPreserveFormatting--) | 指示在刷新或重新计算数据透视表时是否保留单元格格式 ([PivotTableFormat](../../com.aspose.cells/pivottableformat))。 |
| [getPrintDrill()](#getPrintDrill--) | 指定一个布尔值，指示是否应打印钻取指示器。 |
| [getPrintTitles()](#getPrintTitles--) | 指示工作表的打印标题是否基于数据透视表报告进行设置。 |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--) | 指示在打开文件时是否刷新数据。 |
| [getRefreshDate()](#getRefreshDate--) | 获取数据透视表上次刷新时的日期时间。 |
| [getRefreshedByWho()](#getRefreshedByWho--) | 获取上次刷新此数据透视表的用户的名称。 |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--) | 指示在表格形式的透视字段中，行区域的透视项标题是否在每个打印页上重复。 |
| [getRowFields()](#getRowFields--) | 返回当前显示为行字段的 [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)。 |
| [getRowGrand()](#getRowGrand--) | 指示是否显示此数据透视表行的总计。 |
| [getRowHeaderCaption()](#getRowHeaderCaption--) | 获取此数据透视表中行标题的自定义标题。 |
| [getRowRange()](#getRowRange--) | 返回一个 CellArea 对象，表示包含数据透视表报告中行区域的范围。 |
| [getSaveData()](#getSaveData--) | 指示是否将 PivotTable 报表的数据随工作簿一起保存。 |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--) | 指示是否显示此数据透视表列的总计。 |
| [getShowDataTips()](#getShowDataTips--) | 指示是否应为 PivotTable 数据单元格显示工具提示。 |
| [getShowDrill()](#getShowDrill--) | 获取是否显示展开/折叠按钮。 |
| [getShowEmptyCol()](#getShowEmptyCol--) | 指示是否在表中包含空列 |
| [getShowEmptyRow()](#getShowEmptyRow--) | 指示是否在表中包含空行。 |
| [getShowHeaders()](#getShowHeaders--) | 指示是否在 PivotTable 视图的行轴和列轴上显示数据字段标题和透视字段标题。 |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--) | 指定一个布尔值，指示是否应从 PivotTable 工具提示中省略成员属性信息。 |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--) | 指示是否应对数据透视表中的列标题应用样式。 |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--) | 指示是否对列应用条纹格式。 |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--) | 指示是否已应用列格式。 |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--) | 指示是否应对数据透视表中的行标题应用样式。 |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--) | 指示是否已对行应用条纹格式。 |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--) | 指示是否显示数据透视表行的总计。 |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--) | 指示是否在 PivotTable 报表中显示行标题标题；指示是否显示字段标题和筛选下拉列表。 |
| [getShowValuesRow()](#getShowValuesRow--) | 指示是否显示值行。 |
| [getSource()](#getSource--) | 获取此数据透视表的数据源。 |
| [getSource(boolean isOriginal)](#getSource-boolean-) | 获取此数据透视表的数据源。 |
| [getSourceDataConnections()](#getSourceDataConnections--) | 获取外部连接的数据源。 |
| [getSourceType()](#getSourceType--) | 获取数据透视表的数据源类型。 |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--) | 指示是否在 PivotTable 报表中将隐藏的页面字段项包含在行和列的小计、块总计和总计中。 |
| [getTableRange1()](#getTableRange1--) | 返回一个 CellArea 对象，表示包含整个 PivotTable 报表的范围，但不包括页面字段。 |
| [getTableRange2()](#getTableRange2--) | 返回一个 CellArea 对象，表示包含整个 PivotTable 报表的范围，包括页面字段。 |
| [getTag()](#getTag--) | 获取与此 PivotTable 视图关联的用户定义字符串。 |
| [getTopRightArea()](#getTopRightArea--) | 表示 PivotTable 右上角的空白区域（对于 RTL 工作表为左上角）。 |
| [getValuesField()](#getValuesField--) | 获取一个 [PivotField](../../com.aspose.cells/pivotfield) 对象，表示数据透视表中的所有数据字段。 |
| [hasBlankRows()](#hasBlankRows--) | 指示是否添加空白行。 |
| [hashCode()](#hashCode--) |  |
| [isAutoFormat()](#isAutoFormat--) | 指示 PivotTable 报表是否自动格式化。 |
| [isExcel2003Compatible()](#isExcel2003Compatible--) | 指定在刷新 PivotTable 时，PivotTable 是否兼容 Excel2003；如果为 true，则字符串必须小于或等于 255 个字符，如果字符串超过 255 个字符，将被截断；如果为 false，则字符串不受上述限制。 |
| [isGridDropZones()](#isGridDropZones--) | 指示 PivotTable 报表是否显示经典的透视表布局。 |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--) | 指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。 |
| [isSelected()](#isSelected--) | 指示此 PivotTable 是否已被选中。 |
| [move(int row, int column)](#move-int-int-) | 将 PivotTable 移动到工作表中的其他位置。 |
| [move(String destCellName)](#move-java.lang.String-) | 将 PivotTable 移动到工作表中的其他位置。 |
| [moveItem(int region, String[] nodes, boolean absolute, int offset)](#moveItem-int-java.lang.String---boolean-int-) | 将一个项目向上或向下移动。 |
| [moveTo(int row, int column)](#moveTo-int-int-) | 将 PivotTable 移动到工作表中的其他位置。 |
| [moveTo(int sheetIndex, int row, int column)](#moveTo-int-int-int-) | 将 PivotTable 移动到工作表中的其他位置。 |
| [moveTo(String destCellName)](#moveTo-java.lang.String-) | 将 PivotTable 移动到工作表中的其他位置。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | 从数据源刷新 [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) 并计算透视视图的数据和样式。 |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | 从数据源刷新 [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) 并计算透视视图的数据和样式。 |
| [refreshData()](#refreshData--) | 从其数据源刷新数据到透视缓存。 |
| [refreshData(PivotTableRefreshOption option)](#refreshData-com.aspose.cells.PivotTableRefreshOption-) | 使用选项从其数据源刷新透视表的数据和设置。 |
| [removeField(int fieldType, PivotField pivotField)](#removeField-int-com.aspose.cells.PivotField-) | 从特定字段区域移除字段 |
| [removeField(int fieldType, int baseFieldIndex)](#removeField-int-int-) | 从特定透视区域移除字段。 |
| [removeField(int fieldType, String fieldName)](#removeField-int-java.lang.String-) | 从特定字段区域移除字段 |
| [selectArea(CellArea ca)](#selectArea-com.aspose.cells.CellArea-) | 选择透视表视图的区域。 |
| [setAllowMultipleFiltersPerField(boolean value)](#setAllowMultipleFiltersPerField-boolean-) | 指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。 |
| [setAltTextDescription(String value)](#setAltTextDescription-java.lang.String-) | 获取替代文本的描述。 |
| [setAltTextTitle(String value)](#setAltTextTitle-java.lang.String-) | 设置替代文本的标题。 |
| [setAutoFormat(boolean value)](#setAutoFormat-boolean-) | 指示 PivotTable 报表是否自动格式化。 |
| [setAutoFormatType(int value)](#setAutoFormatType-int-) | 设置 PivotTable 的自动格式类型。 |
| [setAutofitColumnWidthOnUpdate(boolean value)](#setAutofitColumnWidthOnUpdate-boolean-) | 指示在更新时是否自动适应列宽 |
| [setColumnGrand(boolean value)](#setColumnGrand-boolean-) | 指示数据透视表报告是否显示列的总计。 |
| [setColumnHeaderCaption(String value)](#setColumnHeaderCaption-java.lang.String-) | 设置 PivotTable 列标题的自定义标题。 |
| [setCustomListSort(boolean value)](#setCustomListSort-boolean-) | 指示在排序数据时是否考虑内置自定义列表 |
| [setDataFieldHeaderName(String value)](#setDataFieldHeaderName-java.lang.String-) | 设置 PivotTable 值区域字段标题的名称。 |
| [setDataSource(String[] value)](#setDataSource-java.lang.String---) | 设置透视表的数据源。 |
| [setDisplayErrorString(boolean value)](#setDisplayErrorString-boolean-) | 指示 PivotTable 报表是否在包含错误的单元格中显示自定义字符串。 |
| [setDisplayImmediateItems(boolean value)](#setDisplayImmediateItems-boolean-) | 指示当 PivotTable 的数据区域为空时，行和列区域中的项目是否可见。 |
| [setDisplayNullString(boolean value)](#setDisplayNullString-boolean-) | 指示 PivotTable 报表在值为 null 时是否显示自定义字符串。 |
| [setEnableDataValueEditing(boolean value)](#setEnableDataValueEditing-boolean-) | 指定一个布尔值，指示是否允许用户编辑 pivottable 数据区域中的单元格。 |
| [setEnableDrilldown(boolean value)](#setEnableDrilldown-boolean-) | 指示是否启用下钻。 |
| [setEnableFieldDialog(boolean value)](#setEnableFieldDialog-boolean-) | 指示当用户双击 PivotTable 字段时，PivotTable 字段对话框是否可用。 |
| [setEnableFieldList(boolean value)](#setEnableFieldList-boolean-) | 指示在 Excel 视图中是否可用 PivotTable 的字段列表。 |
| [setEnableWizard(boolean value)](#setEnableWizard-boolean-) | 指示 PivotTable 向导是否可用。 |
| [setErrorString(String value)](#setErrorString-java.lang.String-) | 获取在 DisplayErrorString 属性为 true 时显示在包含错误的单元格中的字符串。默认值为空字符串。 |
| [setExcel2003Compatible(boolean value)](#setExcel2003Compatible-boolean-) | 指定在刷新 PivotTable 时，PivotTable 是否兼容 Excel2003；如果为 true，则字符串必须小于或等于 255 个字符，如果字符串超过 255 个字符，将被截断；如果为 false，则字符串不受上述限制。 |
| [setFieldListSortAscending(boolean value)](#setFieldListSortAscending-boolean-) | 指示 PivotTable 中的字段在字段列表中是否以非默认顺序排序。 |
| [setGrandTotalName(String value)](#setGrandTotalName-java.lang.String-) | 返回显示在总计列或行标题中的标签。 |
| [setGridDropZones(boolean value)](#setGridDropZones-boolean-) | 指示 PivotTable 报表是否显示经典的透视表布局。 |
| [setHasBlankRows(boolean value)](#setHasBlankRows-boolean-) | 指示是否添加空白行。 |
| [setIndent(int value)](#setIndent-int-) | 指定紧凑轴的缩进增量，可用于将 Report Layout 设置为紧凑形式。 |
| [setItemPrintTitles(boolean value)](#setItemPrintTitles-boolean-) | 指示是否应在每页打印的顶部重复 PivotItem 名称。 |
| [setManualUpdate(boolean value)](#setManualUpdate-boolean-) | 指示 PivotTable 报表是否仅在用户请求时重新计算。 |
| [setMergeLabels(boolean value)](#setMergeLabels-boolean-) | 设置是否合并跨多个单元格的行/列字段标签。 |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | 指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。 |
| [setMultipleFieldFilters(boolean value)](#setMultipleFieldFilters-boolean-) | 指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。 |
| [setName(String value)](#setName-java.lang.String-) | 获取 PivotTable 的名称 |
| [setNullString(String value)](#setNullString-java.lang.String-) | 获取在 DisplayNullString 属性为 true 时显示在包含 null 值的单元格中的字符串。默认值为空字符串。 |
| [setPageFieldOrder(int value)](#setPageFieldOrder-int-) | 设置页面字段添加到 PivotTable 报表布局中的顺序。 |
| [setPageFieldWrapCount(int value)](#setPageFieldWrapCount-int-) | 获取数据透视表报告中每列或每行的页面字段数量。 |
| [setPivotTableStyle(TableStyle value)](#setPivotTableStyle-com.aspose.cells.TableStyle-) | 获取此数据透视表的 [TableStyle](../../com.aspose.cells/tablestyle) 设置。 |
| [setPivotTableStyleName(String value)](#setPivotTableStyleName-java.lang.String-) | 设置透视表的样式名称。 |
| [setPivotTableStyleType(int value)](#setPivotTableStyleType-int-) | 设置内置的透视表样式。 |
| [setPreserveCellFormattingOnUpdate(boolean value)](#setPreserveCellFormattingOnUpdate-boolean-) | 指示在刷新或重新计算数据透视表时是否保留单元格格式 ([PivotTableFormat](../../com.aspose.cells/pivottableformat))。 |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | 指示在刷新或重新计算数据透视表时是否保留单元格格式 ([PivotTableFormat](../../com.aspose.cells/pivottableformat))。 |
| [setPrintDrill(boolean value)](#setPrintDrill-boolean-) | 指定一个布尔值，指示是否应打印钻取指示器。 |
| [setPrintTitles(boolean value)](#setPrintTitles-boolean-) | 指示工作表的打印标题是否基于数据透视表报告进行设置。 |
| [setRefreshDataOnOpeningFile(boolean value)](#setRefreshDataOnOpeningFile-boolean-) | 指示在打开文件时是否刷新数据。 |
| [setRepeatItemsOnEachPrintedPage(boolean value)](#setRepeatItemsOnEachPrintedPage-boolean-) | 指示在表格形式的透视字段中，行区域的透视项标题是否在每个打印页上重复。 |
| [setRowGrand(boolean value)](#setRowGrand-boolean-) | 指示是否显示此数据透视表行的总计。 |
| [setRowHeaderCaption(String value)](#setRowHeaderCaption-java.lang.String-) | 设置此 PivotTable 行标题的自定义标题。 |
| [setSaveData(boolean value)](#setSaveData-boolean-) | 指示是否将 PivotTable 报表的数据随工作簿一起保存。 |
| [setSelected(boolean value)](#setSelected-boolean-) | 指示此 PivotTable 是否已被选中。 |
| [setShowColumnGrandTotals(boolean value)](#setShowColumnGrandTotals-boolean-) | 指示是否显示此数据透视表列的总计。 |
| [setShowDataTips(boolean value)](#setShowDataTips-boolean-) | 指示是否应为 PivotTable 数据单元格显示工具提示。 |
| [setShowDrill(boolean value)](#setShowDrill-boolean-) | 设置是否显示展开/折叠按钮。 |
| [setShowEmptyCol(boolean value)](#setShowEmptyCol-boolean-) | 指示是否在表中包含空列 |
| [setShowEmptyRow(boolean value)](#setShowEmptyRow-boolean-) | 指示是否在表中包含空行。 |
| [setShowHeaders(boolean value)](#setShowHeaders-boolean-) | 指示是否在 PivotTable 视图的行轴和列轴上显示数据字段标题和透视字段标题。 |
| [setShowMemberPropertyTips(boolean value)](#setShowMemberPropertyTips-boolean-) | 指定一个布尔值，指示是否应从 PivotTable 工具提示中省略成员属性信息。 |
| [setShowPivotStyleColumnHeader(boolean value)](#setShowPivotStyleColumnHeader-boolean-) | 指示是否应对数据透视表中的列标题应用样式。 |
| [setShowPivotStyleColumnStripes(boolean value)](#setShowPivotStyleColumnStripes-boolean-) | 指示是否对列应用条纹格式。 |
| [setShowPivotStyleLastColumn(boolean value)](#setShowPivotStyleLastColumn-boolean-) | 指示是否已应用列格式。 |
| [setShowPivotStyleRowHeader(boolean value)](#setShowPivotStyleRowHeader-boolean-) | 指示是否应对数据透视表中的行标题应用样式。 |
| [setShowPivotStyleRowStripes(boolean value)](#setShowPivotStyleRowStripes-boolean-) | 指示是否已对行应用条纹格式。 |
| [setShowRowGrandTotals(boolean value)](#setShowRowGrandTotals-boolean-) | 指示是否显示数据透视表行的总计。 |
| [setShowRowHeaderCaption(boolean value)](#setShowRowHeaderCaption-boolean-) | 指示是否在 PivotTable 报表中显示行标题标题；指示是否显示字段标题和筛选下拉列表。 |
| [setShowValuesRow(boolean value)](#setShowValuesRow-boolean-) | 指示是否显示值行。 |
| [setSubtotalHiddenPageItems(boolean value)](#setSubtotalHiddenPageItems-boolean-) | 指示是否在 PivotTable 报表中将隐藏的页面字段项包含在行和列的小计、块总计和总计中。 |
| [setTag(String value)](#setTag-java.lang.String-) | 设置与此 PivotTable 视图关联的用户定义字符串。 |
| [showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)](#showDetail-int-int-boolean-int-int-) | 在数据区域中显示单个项目的详细信息到新表。 |
| [showInCompactForm()](#showInCompactForm--) | 以紧凑形式布局数据透视表视图。 |
| [showInOutlineForm()](#showInOutlineForm--) | 以大纲形式布局数据透视表。 |
| [showInTabularForm()](#showInTabularForm--) | 以表格形式布局数据透视表。 |
| [showReportFilterPage(PivotField pageField)](#showReportFilterPage-com.aspose.cells.PivotField-) | 根据 PivotField 显示所有报表筛选页面，PivotField 必须位于 PageFields 中。 |
| [showReportFilterPageByIndex(int posIndex)](#showReportFilterPageByIndex-int-) | 根据 PageFields 中的位置索引显示所有报表筛选页面。 |
| [showReportFilterPageByName(String fieldName)](#showReportFilterPageByName-java.lang.String-) | 根据 PivotField 的名称显示所有报表筛选页面，PivotField 必须位于 PageFields 中。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedField(String name, String formula) {#addCalculatedField-java.lang.String-java.lang.String-}
```
public void addCalculatedField(String name, String formula)
```


向数据透视字段添加计算字段并将其拖动到数据区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 计算字段的名称 |
| formula | java.lang.String | 计算字段的公式。 |

### addCalculatedField(String name, String formula, boolean dragToDataArea) {#addCalculatedField-java.lang.String-java.lang.String-boolean-}
```
public void addCalculatedField(String name, String formula, boolean dragToDataArea)
```


向数据透视字段添加计算字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 计算字段的名称 |
| formula | java.lang.String | 计算字段的公式。 |
| dragToDataArea | boolean | True，立即将此字段拖动到数据区域 |

### addFieldToArea(int fieldType, PivotField pivotField) {#addFieldToArea-int-com.aspose.cells.PivotField-}
```
public int addFieldToArea(int fieldType, PivotField pivotField)
```


将字段添加到特定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). 字段区域类型。 |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | 基字段中的字段。 |

**Returns:**
int - 特定字段中的字段位置。
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


将字段添加到特定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). 字段区域类型。 |
| baseFieldIndex | int | 基字段中的索引。 |

**Returns:**
int - 特定字段中的字段位置。
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


将字段添加到特定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). 字段区域类型。 |
| fieldName | java.lang.String | 基字段中的名称。 |

**Returns:**
int - 特定字段中的字段位置。如果不存在相应名称的字段，返回 -1。
### calculateData() {#calculateData--}
```
public void calculateData()
```


将数据透视表的数据计算到单元格。

**Remarks**

此方法仅使用 [getPivotCache()](../../com.aspose.cells/pivottable\\#getPivotCache--) 中的缓存数据进行计算。因此，如果您想使用最新的数据源进行计算，请使用 [PivotCache.refresh()](../../com.aspose.cells/pivotcache\\#refresh--) 方法进行计算。如果仅更改了数据透视表的设置，使用 [calculateData()](../../com.aspose.cells/pivottable\\#calculateData--) 即可。

### calculateData(PivotTableCalculateOption option) {#calculateData-com.aspose.cells.PivotTableCalculateOption-}
```
public PivotTable[] calculateData(PivotTableCalculateOption option)
```


使用选项计算数据透视表。

**Remarks**

如果 [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\\#getRefreshData--) 为 true，则此方法将从数据源刷新透视缓存，然后基于相同的透视缓存计算所有数据透视表。否则，仅使用透视缓存中的缓存数据进行计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../../com.aspose.cells/pivottablecalculateoption) | 计算数据透视表的选项 |

**Returns:**
com.aspose.cells.PivotTable[] - 返回所有已计算的数据透视表。如果 [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\\#getRefreshData--) 为 true，则基于相同透视缓存的所有数据透视表将一起计算。
### calculateRange() {#calculateRange--}
```
public void calculateRange()
```


计算数据透视表的范围。

**Remarks**

如果未调用此方法，可能数据透视表范围不正确。

### changeDataSource(String[] source) {#changeDataSource-java.lang.String---}
```
public void changeDataSource(String[] source)
```


更改数据透视表的数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 源 | java.lang.String[] |  |

### clearAll() {#clearAll--}
```
public void clearAll()
```


从区域中移除所有字段。

### clearData() {#clearData--}
```
public void clearData()
```


清除 PivotTable 视图的数据和格式。

**Remarks**

如果在添加或删除 PivotField 之前未调用此方法，可能 PivotTable 数据未被纠正

### clearFilters() {#clearFilters--}
```
public void clearFilters()
```


清除此数据透视表的所有筛选。

### copyStyle(PivotTable pivotTable) {#copyStyle-com.aspose.cells.PivotTable-}
```
public void copyStyle(PivotTable pivotTable)
```


从另一个数据透视表复制命名样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | 源透视表。 |

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
### exportViewToJson(PivotViewToJsonOptions options) {#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-}
```
public String exportViewToJson(PivotViewToJsonOptions options)
```


将数据透视视图导出为 JSON。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [PivotViewToJsonOptions](../../com.aspose.cells/pivotviewtojsonoptions) |  |

**Returns:**
java.lang.String -
### fields(int fieldType) {#fields-int-}
```
public PivotFieldCollection fields(int fieldType)
```


根据字段类型获取特定字段。

**Remarks**

注意：此方法现已过时。请改用 PivotField.GetFields(PivotFieldType) 方法。此方法将在自 2024 年 5 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。字段类型。 |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific field collection
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


格式化数据透视表的选定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 单元格的范围。 |
| style | [Style](../../com.aspose.cells/style) | 样式 |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


格式化数据透视表的选定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | 选定的透视视图区域。 |
| style | [Style](../../com.aspose.cells/style) | 已格式化的设置。 |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


格式化数据透视表区域中的单元格

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 单元格的行索引 |
| 列 | int | 单元格的列索引 |
| style | [Style](../../com.aspose.cells/style) | 用于格式化单元格的样式 |

### formatAll(Style style) {#formatAll-com.aspose.cells.Style-}
```
public void formatAll(Style style)
```


格式化数据透视表区域中的所有单元格

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 用于格式化的样式 |

### formatRow(int row, Style style) {#formatRow-int-com.aspose.cells.Style-}
```
public void formatRow(int row, Style style)
```


格式化数据透视表区域中的行数据

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | Row 对象的行索引 |
| style | [Style](../../com.aspose.cells/style) | 用于格式化的样式 |

### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```
public boolean getAllowMultipleFiltersPerField()
```


指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。

**Returns:**
boolean
### getAltTextDescription() {#getAltTextDescription--}
```
public String getAltTextDescription()
```


获取替代文本的描述。

**Returns:**
java.lang.String
### getAltTextTitle() {#getAltTextTitle--}
```
public String getAltTextTitle()
```


获取替代文本的标题。

**Returns:**
java.lang.String
### getAutoFormatType() {#getAutoFormatType--}
```
public int getAutoFormatType()
```


获取数据透视表的自动格式类型。

参见 [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype)。

**Returns:**
int
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```
public boolean getAutofitColumnWidthOnUpdate()
```


指示在更新时是否自动适应列宽

**Returns:**
boolean
### getBaseFields() {#getBaseFields--}
```
public PivotFieldCollection getBaseFields()
```


返回数据透视表中的所有基础数据透视字段。

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getButtonArea(int axisType) {#getButtonArea-int-}
```
public CellArea getButtonArea(int axisType)
```


获取包含字段按钮的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。区域类型。 |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - 
### getCellByDisplayName(String displayName) {#getCellByDisplayName-java.lang.String-}
```
public Cell getCellByDisplayName(String displayName)
```


通过 PivotField 的显示名称获取 [Cell](../../com.aspose.cells/cell) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| displayName | java.lang.String | PivotField 的 DisplayName |

**Returns:**
[Cell](../../com.aspose.cells/cell) - the Cell object
### getChildren() {#getChildren--}
```
public PivotTable[] getChildren()
```


获取使用此数据透视表数据作为数据源的子数据透视表。

**Remarks**

注意：此方法现已过时。请改用 PivotTable.GetDependentPivotTables() 方法。此方法将在自 2026 年 4 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
com.aspose.cells.PivotTable[] - PivotTable 数组对象
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnFields() {#getColumnFields--}
```
public PivotFieldCollection getColumnFields()
```


返回当前显示为列字段的 PivotFields 对象。

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getColumnGrand() {#getColumnGrand--}
```
public boolean getColumnGrand()
```


指示数据透视表报告是否显示列的总计。

**Remarks**

注意：此属性现已过时。请改用 PivotTable.ShowColumnGrandTotals 方法。此方法将在自 2024 年 12 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```
public String getColumnHeaderCaption()
```


获取数据透视表列标题的自定义标题。

**Returns:**
java.lang.String
### getColumnRange() {#getColumnRange--}
```
public CellArea getColumnRange()
```


返回一个 CellArea 对象，表示包含 PivotTable 报表中列区域的范围。只读。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getConditionalFormats() {#getConditionalFormats--}
```
public PivotConditionalFormatCollection getConditionalFormats()
```


获取数据透视表的条件格式。

**Returns:**
[PivotConditionalFormatCollection](../../com.aspose.cells/pivotconditionalformatcollection)
### getCustomListSort() {#getCustomListSort--}
```
public boolean getCustomListSort()
```


指示在排序数据时是否考虑内置自定义列表

**Returns:**
boolean
### getDataBodyRange() {#getDataBodyRange--}
```
public CellArea getDataBodyRange()
```


返回一个 [CellArea](../../com.aspose.cells/cellarea) 对象，表示在列表中位于标题行和插入行之间的数据区域的范围。只读。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getDataField() {#getDataField--}
```
public PivotField getDataField()
```


获取一个 [PivotField](../../com.aspose.cells/pivotfield) 对象，表示 PivotTable 中的所有数据字段。只读。当 Data 区域中有两个或更多数据字段时才会创建。默认位于行区域。您可以使用 PivotTable.AddFieldToArea() 方法将其拖动到行/列区域。

**Remarks**

注意：此方法现已过时。请改用 PivotTable.ValuesField 属性。此方法将在自 2025 年 10 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```
public String getDataFieldHeaderName()
```


获取 PivotTable 中值区域字段标题的名称。

**Returns:**
java.lang.String
### getDataFields() {#getDataFields--}
```
public PivotFieldCollection getDataFields()
```


获取一个 [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)，它表示 PivotTable 中的所有数据字段。

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getDataSource() {#getDataSource--}
```
public String[] getDataSource()
```


获取 PivotTable 的数据源。

**Returns:**
java.lang.String[]
### getDependentPivotTables() {#getDependentPivotTables--}
```
public PivotTable[] getDependentPivotTables()
```


获取所有使用此 PivotTable 作为数据源的 [PivotTable](../../com.aspose.cells/pivottable)s。

**Remarks**

因为透视表可能相互依赖数据，必须按正确顺序刷新以确保数据一致性。

**Returns:**
com.aspose.cells.PivotTable[] -
### getDisplayErrorString() {#getDisplayErrorString--}
```
public boolean getDisplayErrorString()
```


指示 PivotTable 报表是否在包含错误的单元格中显示自定义字符串。

**Returns:**
boolean
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```
public boolean getDisplayImmediateItems()
```


指示当 PivotTable 的数据区域为空时，行和列区域中的项目是否可见。默认值为 true。

**Returns:**
boolean
### getDisplayNullString() {#getDisplayNullString--}
```
public boolean getDisplayNullString()
```


指示 PivotTable 报表在值为 null 时是否显示自定义字符串。

**Returns:**
boolean
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```
public boolean getEnableDataValueEditing()
```


指定一个布尔值，指示是否允许用户编辑 pivottable 数据区域中的单元格。默认值为 false。

**Returns:**
boolean
### getEnableDrilldown() {#getEnableDrilldown--}
```
public boolean getEnableDrilldown()
```


指示是否启用下钻。

**Returns:**
boolean
### getEnableFieldDialog() {#getEnableFieldDialog--}
```
public boolean getEnableFieldDialog()
```


指示当用户双击 PivotTable 字段时，PivotTable 字段对话框是否可用。

**Returns:**
boolean
### getEnableFieldList() {#getEnableFieldList--}
```
public boolean getEnableFieldList()
```


指示在 Excel 视图中是否可用 PivotTable 的字段列表。

**Returns:**
boolean
### getEnableWizard() {#getEnableWizard--}
```
public boolean getEnableWizard()
```


指示 PivotTable 向导是否可用。

**Returns:**
boolean
### getErrorString() {#getErrorString--}
```
public String getErrorString()
```


获取在 DisplayErrorString 属性为 true 时显示在包含错误的单元格中的字符串。默认值为空字符串。

**Returns:**
java.lang.String
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```
public ExternalConnection getExternalConnectionDataSource()
```


获取外部连接数据源。

**Remarks**

注意：此属性已过时。请改用 PivotTable.GetSourceDataConnections() 方法。该方法将在自 2024 年 10 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getFieldListSortAscending() {#getFieldListSortAscending--}
```
public boolean getFieldListSortAscending()
```


指示 PivotTable 中的字段在字段列表中是否以非默认顺序排序。

**Returns:**
boolean
### getFields(int fieldType) {#getFields-int-}
```
public PivotFieldCollection getFields(int fieldType)
```


按区域获取特定的 pivot field 列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。区域类型。 |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific pivot field collection
### getFilterArea() {#getFilterArea--}
```
public CellArea getFilterArea()
```


获取筛选区域的范围。

**Remarks**

仅在存在筛选透视字段时有效。如果此 pivot table 不包含筛选透视字段，将返回空区域。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getGrandTotalName() {#getGrandTotalName--}
```
public String getGrandTotalName()
```


返回在总计列或行标题中显示的标签。默认值为字符串 "Grand Total"。

**Returns:**
java.lang.String
### getHorizontalBreaks() {#getHorizontalBreaks--}
```
public ArrayList getHorizontalBreaks()
```


获取 PivotTable 水平分页符的行索引列表。

**Remarks**

注意：此方法已过时。请改用 PivotTable.GetHorizontalPageBreaks() 方法。该方法将在自 2024 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.util.ArrayList -
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public int[] getHorizontalPageBreaks()
```


获取此 PivotTable 的水平分页符。

**Returns:**
int[] -
### getIndent() {#getIndent--}
```
public int getIndent()
```


指定紧凑轴的缩进增量，可用于将 Report Layout 设置为紧凑形式。

**Returns:**
int
### getItemPrintTitles() {#getItemPrintTitles--}
```
public boolean getItemPrintTitles()
```


指示是否应在每页打印的顶部重复 PivotItem 名称。

**Remarks**

注意：此属性已过时。请改用 PivotTable.RepeatItemsOnEachPrintedPage 属性。该方法将在自 2024 年 10 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getManualUpdate() {#getManualUpdate--}
```
public boolean getManualUpdate()
```


指示 PivotTable 报表是否仅在用户请求时重新计算。

**Returns:**
boolean
### getMergeLabels() {#getMergeLabels--}
```
public boolean getMergeLabels()
```


获取是否合并跨多个单元格的行/列字段标签。

**Returns:**
boolean
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。

参见 [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype)。

**Remarks**

注意：此属性已过时。请改用 PivotCache.MissingItemsLimit 属性。该方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


获取 PivotTable 的名称

**Returns:**
java.lang.String
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
```
public String[] getNamesOfSourceDataConnections()
```


获取外部源数据连接的名称。

**Returns:**
java.lang.String[]
### getNullString() {#getNullString--}
```
public String getNullString()
```


获取在 DisplayNullString 属性为 true 时显示在包含 null 值的单元格中的字符串。默认值为空字符串。

**Returns:**
java.lang.String
### getPageFieldOrder() {#getPageFieldOrder--}
```
public int getPageFieldOrder()
```


获取页面字段添加到数据透视表报告布局中的顺序。

参见 [PrintOrderType](../../com.aspose.cells/printordertype)。

**Returns:**
int
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```
public int getPageFieldWrapCount()
```


获取数据透视表报告中每列或每行的页面字段数量。

**Returns:**
int
### getPageFields() {#getPageFields--}
```
public PivotFieldCollection getPageFields()
```


返回当前显示为页面字段的 [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)。

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getPivotCache() {#getPivotCache--}
```
public PivotCache getPivotCache()
```


获取数据源。

**Returns:**
[PivotCache](../../com.aspose.cells/pivotcache)
### getPivotFilters() {#getPivotFilters--}
```
public PivotFilterCollection getPivotFilters()
```


返回数据透视表中的所有筛选器。

**Returns:**
[PivotFilterCollection](../../com.aspose.cells/pivotfiltercollection)
### getPivotFormatConditions() {#getPivotFormatConditions--}
```
public PivotFormatConditionCollection getPivotFormatConditions()
```


获取数据透视表的格式条件。

**Remarks**

注意：此属性已过时。请改用 PivotTable.ConditionalFormats 属性。该方法将在自 2024 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[PivotFormatConditionCollection](../../com.aspose.cells/pivotformatconditioncollection)
### getPivotFormats() {#getPivotFormats--}
```
public PivotTableFormatCollection getPivotFormats()
```


获取应用于此数据透视表的所有单元格格式。

**Returns:**
[PivotTableFormatCollection](../../com.aspose.cells/pivottableformatcollection)
### getPivotTableStyle() {#getPivotTableStyle--}
```
public TableStyle getPivotTableStyle()
```


获取此数据透视表的 [TableStyle](../../com.aspose.cells/tablestyle) 设置。

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle)
### getPivotTableStyleName() {#getPivotTableStyleName--}
```
public String getPivotTableStyleName()
```


获取数据透视表的样式名称。

**Returns:**
java.lang.String
### getPivotTableStyleType() {#getPivotTableStyleType--}
```
public int getPivotTableStyleType()
```


获取内置的数据透视表样式。

参见 [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype)。

**Returns:**
int
### getPivotTablesWithSamePivotCache() {#getPivotTablesWithSamePivotCache--}
```
public PivotTable[] getPivotTablesWithSamePivotCache()
```


获取具有相同数据透视缓存的所有数据透视表。

**Returns:**
com.aspose.cells.PivotTable[] -
### getPreserveCellFormattingOnUpdate() {#getPreserveCellFormattingOnUpdate--}
```
public boolean getPreserveCellFormattingOnUpdate()
```


指示在刷新或重新计算数据透视表时是否保留单元格格式 ([PivotTableFormat](../../com.aspose.cells/pivottableformat))。

**Returns:**
boolean
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


指示在刷新或重新计算数据透视表时是否保留单元格格式 ([PivotTableFormat](../../com.aspose.cells/pivottableformat))。

**Remarks**

注意：此属性已过时。请改用 PivotTable.PreserveCellFormattingOnUpdate 属性。该方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getPrintDrill() {#getPrintDrill--}
```
public boolean getPrintDrill()
```


指定一个布尔值，指示是否应打印钻取指示器。当在 pivottable 上显示时，打印展开/折叠按钮。

**Returns:**
boolean
### getPrintTitles() {#getPrintTitles--}
```
public boolean getPrintTitles()
```


指示是否根据 PivotTable 报表设置工作表的打印标题。默认值为 false。

**Returns:**
boolean
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```
public boolean getRefreshDataOnOpeningFile()
```


指示在打开文件时是否刷新数据。

**Returns:**
boolean
### getRefreshDate() {#getRefreshDate--}
```
public DateTime getRefreshDate()
```


获取数据透视表上次刷新时的日期时间。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getRefreshedByWho() {#getRefreshedByWho--}
```
public String getRefreshedByWho()
```


获取上次刷新此数据透视表的用户的名称。

**Returns:**
java.lang.String
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```
public boolean getRepeatItemsOnEachPrintedPage()
```


指示在表格形式的透视字段中，行区域的透视项标题是否在每个打印页上重复。

**Returns:**
boolean
### getRowFields() {#getRowFields--}
```
public PivotFieldCollection getRowFields()
```


返回当前显示为行字段的 [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)。

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getRowGrand() {#getRowGrand--}
```
public boolean getRowGrand()
```


指示是否显示此数据透视表行的总计。

**Remarks**

注意：此属性已过时。请改用 PivotTable.ShowRowGrandTotals 方法。该方法将在自 2024 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getRowHeaderCaption() {#getRowHeaderCaption--}
```
public String getRowHeaderCaption()
```


获取此数据透视表中行标题的自定义标题。

**Returns:**
java.lang.String
### getRowRange() {#getRowRange--}
```
public CellArea getRowRange()
```


返回一个 CellArea 对象，表示在 PivotTable 报表中包含行区域的范围。只读。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


指示是否将 PivotTable 报表的数据随工作簿一起保存。

**Returns:**
boolean
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```
public boolean getShowColumnGrandTotals()
```


指示是否显示此数据透视表列的总计。

**Returns:**
boolean
### getShowDataTips() {#getShowDataTips--}
```
public boolean getShowDataTips()
```


指示是否应为 PivotTable 数据单元格显示工具提示。

**Returns:**
boolean
### getShowDrill() {#getShowDrill--}
```
public boolean getShowDrill()
```


获取是否显示展开/折叠按钮。

**Returns:**
boolean
### getShowEmptyCol() {#getShowEmptyCol--}
```
public boolean getShowEmptyCol()
```


指示是否在表中包含空列

**Returns:**
boolean
### getShowEmptyRow() {#getShowEmptyRow--}
```
public boolean getShowEmptyRow()
```


指示是否在表中包含空行。

**Returns:**
boolean
### getShowHeaders() {#getShowHeaders--}
```
public boolean getShowHeaders()
```


指示是否在 PivotTable 视图的行轴和列轴上显示数据字段标题和透视字段标题。

**Returns:**
boolean
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```
public boolean getShowMemberPropertyTips()
```


指定一个布尔值，指示是否应从 PivotTable 工具提示中省略成员属性信息。

**Returns:**
boolean
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```
public boolean getShowPivotStyleColumnHeader()
```


指示是否应对数据透视表中的列标题应用样式。

**Returns:**
boolean
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```
public boolean getShowPivotStyleColumnStripes()
```


指示是否对列应用条纹格式。

**Returns:**
boolean
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```
public boolean getShowPivotStyleLastColumn()
```


指示是否已应用列格式。

**Returns:**
boolean
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```
public boolean getShowPivotStyleRowHeader()
```


指示是否应对数据透视表中的行标题应用样式。

**Returns:**
boolean
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```
public boolean getShowPivotStyleRowStripes()
```


指示是否已对行应用条纹格式。

**Returns:**
boolean
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```
public boolean getShowRowGrandTotals()
```


指示是否显示数据透视表行的总计。

**Remarks**

**Returns:**
boolean
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```
public boolean getShowRowHeaderCaption()
```


指示是否在 PivotTable 报表中显示行标题标题；指示是否显示字段标题和筛选下拉列表。

**Remarks**

注意：此属性已过时。请改用 PivotTable.ShowHeaders 属性。该方法将在自 2026 年 4 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getShowValuesRow() {#getShowValuesRow--}
```
public boolean getShowValuesRow()
```


指示是否显示值行。

**Returns:**
boolean
### getSource() {#getSource--}
```
public String[] getSource()
```


获取此数据透视表的数据源。

**Returns:**
java.lang.String[]
### getSource(boolean isOriginal) {#getSource-boolean-}
```
public String[] getSource(boolean isOriginal)
```


获取此数据透视表的数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isOriginal | boolean | 指示是返回原始数据还是显示数据源。 |

**Returns:**
java.lang.String[] -
### getSourceDataConnections() {#getSourceDataConnections--}
```
public ExternalConnection[] getSourceDataConnections()
```


获取外部连接的数据源。

**Returns:**
com.aspose.cells.ExternalConnection[]
### getSourceType() {#getSourceType--}
```
public byte getSourceType()
```


获取数据透视表的数据源类型。

参见 [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype)。

**Returns:**
byte
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```
public boolean getSubtotalHiddenPageItems()
```


指示在 PivotTable 报表中是否将隐藏的页面字段项包含在行和列小计、区块总计以及总计中。默认值为 False。

**Returns:**
boolean
### getTableRange1() {#getTableRange1--}
```
public CellArea getTableRange1()
```


返回一个 CellArea 对象，表示包含整个数据透视表报告的范围，但不包括页面字段。只读。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTableRange2() {#getTableRange2--}
```
public CellArea getTableRange2()
```


返回一个 CellArea 对象，表示包含整个数据透视表报告的范围，包括页面字段。只读。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTag() {#getTag--}
```
public String getTag()
```


获取与此 PivotTable 视图关联的用户定义字符串。

**Returns:**
java.lang.String
### getTopRightArea() {#getTopRightArea--}
```
public CellArea getTopRightArea()
```


表示 PivotTable 右上角的空白区域（对于 RTL 工作表为左上角）。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getValuesField() {#getValuesField--}
```
public PivotField getValuesField()
```


获取一个 [PivotField](../../com.aspose.cells/pivotfield) 对象，表示 PivotTable 中的所有数据字段。只读。当 Data 区域中有两个或更多数据字段时才会创建。默认位于行区域。您可以使用 PivotTable.AddFieldToArea() 方法将其拖动到行/列区域。

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### hasBlankRows() {#hasBlankRows--}
```
public boolean hasBlankRows()
```


指示是否添加空白行。此属性仅适用于需要添加空白行的数据透视表自动格式类型。

**Remarks**

注意：此属性已过时。请改用 PivotField.InsertBlankRow 属性。此方法将在自 2026 年 4 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFormat() {#isAutoFormat--}
```
public boolean isAutoFormat()
```


指示数据透视表报告是否自动格式化。复选框 “autoformat table”，位于 Excel 2003 的数据透视表选项中。

**Returns:**
boolean
### isExcel2003Compatible() {#isExcel2003Compatible--}
```
public boolean isExcel2003Compatible()
```


指定在刷新数据透视表时，数据透视表是否兼容 Excel2003。如果为 true，则字符串必须小于或等于 255 个字符，超过 255 个字符的将被截断。如果为 false，则字符串不受上述限制。默认值为 true。

**Returns:**
boolean
### isGridDropZones() {#isGridDropZones--}
```
public boolean isGridDropZones()
```


指示数据透视表报告是否显示经典数据透视表布局。（在网格中启用字段拖动）

**Returns:**
boolean
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```
public boolean isMultipleFieldFilters()
```


指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。

**Remarks**

注意：此属性已过时。请改用 PivotTable.AllowMultipleFiltersPerField 属性。此方法将在自 2024 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


指示此 PivotTable 是否已被选中。

**Returns:**
boolean
### move(int row, int column) {#move-int-int-}
```
public void move(int row, int column)
```


将 PivotTable 移动到工作表中的其他位置。

**Remarks**

注意：此属性已过时。请改用 PivotTable.MoveTo() 方法。此方法将在自 2024 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

### move(String destCellName) {#move-java.lang.String-}
```
public void move(String destCellName)
```


将 PivotTable 移动到工作表中的其他位置。

**Remarks**

注意：此属性已过时。请改用 PivotTable.MoveTo() 方法。此方法将在自 2024 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destCellName | java.lang.String | 目标单元格名称。 |

### moveItem(int region, String[] nodes, boolean absolute, int offset) {#moveItem-int-java.lang.String---boolean-int-}
```
public void moveItem(int region, String[] nodes, boolean absolute, int offset)
```


将一个项目向上或向下移动。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| region | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。区域。仅用于行或列。 |
| 节点 | java.lang.String[] | 该项。 |
| 绝对 | boolean | 指示偏移是否为绝对位置。 |
| 偏移 | int | 如果 absolute 为 true：0 移动到开头，-1 移动到结尾，其他值表示绝对位置；否则 offset 为相对位置。 |

### moveTo(int row, int column) {#moveTo-int-int-}
```
public void moveTo(int row, int column)
```


将 PivotTable 移动到工作表中的其他位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

### moveTo(int sheetIndex, int row, int column) {#moveTo-int-int-int-}
```
public void moveTo(int sheetIndex, int row, int column)
```


将 PivotTable 移动到工作表中的其他位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 目标工作表的索引 |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

### moveTo(String destCellName) {#moveTo-java.lang.String-}
```
public void moveTo(String destCellName)
```


将 PivotTable 移动到工作表中的其他位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destCellName | java.lang.String | 目标单元格名称。 |

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
public int refresh()
```


从数据源刷新 [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) 并计算透视视图的数据和样式。

**Remarks**

所有依赖相同 PivotCache 的数据透视表将被重新计算。

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate)。
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


从数据源刷新 [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) 并计算透视视图的数据和样式。

**Remarks**

所有依赖相同 PivotCache 的数据透视表将被重新计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate)。
### refreshData() {#refreshData--}
```
public int refreshData()
```


从其数据源刷新数据到透视缓存。

**Remarks**

我们将从数据源收集数据到 PivotCache，然后将缓存中的数据计算到单元格。最好直接调用 [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) 来刷新并计算文件中的所有数据透视表，而不是逐个刷新。注意：此方法已过时。请改用 [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) 方法，并移除随后使用的 [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) ，因为在刷新 [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) 时该数据透视表将被计算。此方法将在自 2026 年 6 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### refreshData(PivotTableRefreshOption option) {#refreshData-com.aspose.cells.PivotTableRefreshOption-}
```
public int refreshData(PivotTableRefreshOption option)
```


使用选项从其数据源刷新透视表的数据和设置。

**Remarks**

我们将从数据源收集数据到 PivotCache，然后将缓存中的数据计算到单元格。最好直接调用 [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) 来刷新并计算文件中的所有数据透视表，而不是逐个刷新。注意：此方法已过时。请改用 [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) 方法，并移除随后使用的 [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) ，因为在刷新 [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) 时该数据透视表将被计算。此方法将在自 2026 年 6 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | 刷新数据透视表数据源的选项。 |

**Returns:**
int
### removeField(int fieldType, PivotField pivotField) {#removeField-int-com.aspose.cells.PivotField-}
```
public void removeField(int fieldType, PivotField pivotField)
```


从特定字段区域移除字段

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). 字段区域类型。 |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | 基字段中的字段。 |

### removeField(int fieldType, int baseFieldIndex) {#removeField-int-int-}
```
public void removeField(int fieldType, int baseFieldIndex)
```


从特定透视区域移除字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). 字段区域类型。 |
| baseFieldIndex | int | 基字段中的字段索引。 |

### removeField(int fieldType, String fieldName) {#removeField-int-java.lang.String-}
```
public void removeField(int fieldType, String fieldName)
```


从特定字段区域移除字段

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). 字段区域类型。 |
| fieldName | java.lang.String | 基字段中的名称。 |

### selectArea(CellArea ca) {#selectArea-com.aspose.cells.CellArea-}
```
public PivotAreaCollection selectArea(CellArea ca)
```


选择透视表视图的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 单元格区域。 |

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection) - 
### setAllowMultipleFiltersPerField(boolean value) {#setAllowMultipleFiltersPerField-boolean-}
```
public void setAllowMultipleFiltersPerField(boolean value)
```


指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAltTextDescription(String value) {#setAltTextDescription-java.lang.String-}
```
public void setAltTextDescription(String value)
```


获取替代文本的描述。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAltTextTitle(String value) {#setAltTextTitle-java.lang.String-}
```
public void setAltTextTitle(String value)
```


设置替代文本的标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAutoFormat(boolean value) {#setAutoFormat-boolean-}
```
public void setAutoFormat(boolean value)
```


指示数据透视表报告是否自动格式化。复选框 “autoformat table”，位于 Excel 2003 的数据透视表选项中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoFormatType(int value) {#setAutoFormatType-int-}
```
public void setAutoFormatType(int value)
```


设置 PivotTable 的自动格式类型。

参见 [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setAutofitColumnWidthOnUpdate(boolean value) {#setAutofitColumnWidthOnUpdate-boolean-}
```
public void setAutofitColumnWidthOnUpdate(boolean value)
```


指示在更新时是否自动适应列宽

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setColumnGrand(boolean value) {#setColumnGrand-boolean-}
```
public void setColumnGrand(boolean value)
```


指示数据透视表报告是否显示列的总计。

**Remarks**

注意：此属性现已过时。请改用 PivotTable.ShowColumnGrandTotals 方法。此方法将在自 2024 年 12 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setColumnHeaderCaption(String value) {#setColumnHeaderCaption-java.lang.String-}
```
public void setColumnHeaderCaption(String value)
```


设置 PivotTable 列标题的自定义标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCustomListSort(boolean value) {#setCustomListSort-boolean-}
```
public void setCustomListSort(boolean value)
```


指示在排序数据时是否考虑内置自定义列表

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDataFieldHeaderName(String value) {#setDataFieldHeaderName-java.lang.String-}
```
public void setDataFieldHeaderName(String value)
```


设置 PivotTable 值区域字段标题的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDataSource(String[] value) {#setDataSource-java.lang.String---}
```
public void setDataSource(String[] value)
```


设置透视表的数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String[] |  |

### setDisplayErrorString(boolean value) {#setDisplayErrorString-boolean-}
```
public void setDisplayErrorString(boolean value)
```


指示 PivotTable 报表是否在包含错误的单元格中显示自定义字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDisplayImmediateItems(boolean value) {#setDisplayImmediateItems-boolean-}
```
public void setDisplayImmediateItems(boolean value)
```


指示当 PivotTable 的数据区域为空时，行和列区域中的项目是否可见。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDisplayNullString(boolean value) {#setDisplayNullString-boolean-}
```
public void setDisplayNullString(boolean value)
```


指示 PivotTable 报表在值为 null 时是否显示自定义字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableDataValueEditing(boolean value) {#setEnableDataValueEditing-boolean-}
```
public void setEnableDataValueEditing(boolean value)
```


指定一个布尔值，指示是否允许用户编辑 pivottable 数据区域中的单元格。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableDrilldown(boolean value) {#setEnableDrilldown-boolean-}
```
public void setEnableDrilldown(boolean value)
```


指示是否启用下钻。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableFieldDialog(boolean value) {#setEnableFieldDialog-boolean-}
```
public void setEnableFieldDialog(boolean value)
```


指示当用户双击 PivotTable 字段时，PivotTable 字段对话框是否可用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableFieldList(boolean value) {#setEnableFieldList-boolean-}
```
public void setEnableFieldList(boolean value)
```


指示在 Excel 视图中是否可用 PivotTable 的字段列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableWizard(boolean value) {#setEnableWizard-boolean-}
```
public void setEnableWizard(boolean value)
```


指示 PivotTable 向导是否可用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setErrorString(String value) {#setErrorString-java.lang.String-}
```
public void setErrorString(String value)
```


获取在 DisplayErrorString 属性为 true 时显示在包含错误的单元格中的字符串。默认值为空字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setExcel2003Compatible(boolean value) {#setExcel2003Compatible-boolean-}
```
public void setExcel2003Compatible(boolean value)
```


指定在刷新数据透视表时，数据透视表是否兼容 Excel2003。如果为 true，则字符串必须小于或等于 255 个字符，超过 255 个字符的将被截断。如果为 false，则字符串不受上述限制。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFieldListSortAscending(boolean value) {#setFieldListSortAscending-boolean-}
```
public void setFieldListSortAscending(boolean value)
```


指示 PivotTable 中的字段在字段列表中是否以非默认顺序排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setGrandTotalName(String value) {#setGrandTotalName-java.lang.String-}
```
public void setGrandTotalName(String value)
```


返回在总计列或行标题中显示的标签。默认值为字符串 "Grand Total"。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setGridDropZones(boolean value) {#setGridDropZones-boolean-}
```
public void setGridDropZones(boolean value)
```


指示数据透视表报告是否显示经典数据透视表布局。（在网格中启用字段拖动）

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasBlankRows(boolean value) {#setHasBlankRows-boolean-}
```
public void setHasBlankRows(boolean value)
```


指示是否添加空白行。此属性仅适用于需要添加空白行的数据透视表自动格式类型。

**Remarks**

注意：此属性已过时。请改用 PivotField.InsertBlankRow 属性。此方法将在自 2026 年 4 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIndent(int value) {#setIndent-int-}
```
public void setIndent(int value)
```


指定紧凑轴的缩进增量，可用于将 Report Layout 设置为紧凑形式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setItemPrintTitles(boolean value) {#setItemPrintTitles-boolean-}
```
public void setItemPrintTitles(boolean value)
```


指示是否应在每页打印的顶部重复 PivotItem 名称。

**Remarks**

注意：此属性已过时。请改用 PivotTable.RepeatItemsOnEachPrintedPage 属性。该方法将在自 2024 年 10 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setManualUpdate(boolean value) {#setManualUpdate-boolean-}
```
public void setManualUpdate(boolean value)
```


指示 PivotTable 报表是否仅在用户请求时重新计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMergeLabels(boolean value) {#setMergeLabels-boolean-}
```
public void setMergeLabels(boolean value)
```


设置是否合并跨多个单元格的行/列字段标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。

参见 [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype)。

**Remarks**

注意：此属性已过时。请改用 PivotCache.MissingItemsLimit 属性。该方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMultipleFieldFilters(boolean value) {#setMultipleFieldFilters-boolean-}
```
public void setMultipleFieldFilters(boolean value)
```


指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。

**Remarks**

注意：此属性已过时。请改用 PivotTable.AllowMultipleFiltersPerField 属性。此方法将在自 2024 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


获取 PivotTable 的名称

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNullString(String value) {#setNullString-java.lang.String-}
```
public void setNullString(String value)
```


获取在 DisplayNullString 属性为 true 时显示在包含 null 值的单元格中的字符串。默认值为空字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPageFieldOrder(int value) {#setPageFieldOrder-int-}
```
public void setPageFieldOrder(int value)
```


设置页面字段添加到 PivotTable 报表布局中的顺序。

参见 [PrintOrderType](../../com.aspose.cells/printordertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPageFieldWrapCount(int value) {#setPageFieldWrapCount-int-}
```
public void setPageFieldWrapCount(int value)
```


获取数据透视表报告中每列或每行的页面字段数量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPivotTableStyle(TableStyle value) {#setPivotTableStyle-com.aspose.cells.TableStyle-}
```
public void setPivotTableStyle(TableStyle value)
```


获取此数据透视表的 [TableStyle](../../com.aspose.cells/tablestyle) 设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TableStyle](../../com.aspose.cells/tablestyle) |  |

### setPivotTableStyleName(String value) {#setPivotTableStyleName-java.lang.String-}
```
public void setPivotTableStyleName(String value)
```


设置透视表的样式名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPivotTableStyleType(int value) {#setPivotTableStyleType-int-}
```
public void setPivotTableStyleType(int value)
```


设置内置的透视表样式。

参见 [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPreserveCellFormattingOnUpdate(boolean value) {#setPreserveCellFormattingOnUpdate-boolean-}
```
public void setPreserveCellFormattingOnUpdate(boolean value)
```


指示在刷新或重新计算数据透视表时是否保留单元格格式 ([PivotTableFormat](../../com.aspose.cells/pivottableformat))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


指示在刷新或重新计算数据透视表时是否保留单元格格式 ([PivotTableFormat](../../com.aspose.cells/pivottableformat))。

**Remarks**

注意：此属性已过时。请改用 PivotTable.PreserveCellFormattingOnUpdate 属性。该方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPrintDrill(boolean value) {#setPrintDrill-boolean-}
```
public void setPrintDrill(boolean value)
```


指定一个布尔值，指示是否应打印钻取指示器。当在 pivottable 上显示时，打印展开/折叠按钮。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPrintTitles(boolean value) {#setPrintTitles-boolean-}
```
public void setPrintTitles(boolean value)
```


指示是否根据 PivotTable 报表设置工作表的打印标题。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRefreshDataOnOpeningFile(boolean value) {#setRefreshDataOnOpeningFile-boolean-}
```
public void setRefreshDataOnOpeningFile(boolean value)
```


指示在打开文件时是否刷新数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRepeatItemsOnEachPrintedPage(boolean value) {#setRepeatItemsOnEachPrintedPage-boolean-}
```
public void setRepeatItemsOnEachPrintedPage(boolean value)
```


指示在表格形式的透视字段中，行区域的透视项标题是否在每个打印页上重复。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRowGrand(boolean value) {#setRowGrand-boolean-}
```
public void setRowGrand(boolean value)
```


指示是否显示此数据透视表行的总计。

**Remarks**

注意：此属性已过时。请改用 PivotTable.ShowRowGrandTotals 方法。该方法将在自 2024 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRowHeaderCaption(String value) {#setRowHeaderCaption-java.lang.String-}
```
public void setRowHeaderCaption(String value)
```


设置此 PivotTable 行标题的自定义标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


指示是否将 PivotTable 报表的数据随工作簿一起保存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


指示此 PivotTable 是否已被选中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowColumnGrandTotals(boolean value) {#setShowColumnGrandTotals-boolean-}
```
public void setShowColumnGrandTotals(boolean value)
```


指示是否显示此数据透视表列的总计。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowDataTips(boolean value) {#setShowDataTips-boolean-}
```
public void setShowDataTips(boolean value)
```


指示是否应为 PivotTable 数据单元格显示工具提示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowDrill(boolean value) {#setShowDrill-boolean-}
```
public void setShowDrill(boolean value)
```


设置是否显示展开/折叠按钮。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowEmptyCol(boolean value) {#setShowEmptyCol-boolean-}
```
public void setShowEmptyCol(boolean value)
```


指示是否在表中包含空列

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowEmptyRow(boolean value) {#setShowEmptyRow-boolean-}
```
public void setShowEmptyRow(boolean value)
```


指示是否在表中包含空行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowHeaders(boolean value) {#setShowHeaders-boolean-}
```
public void setShowHeaders(boolean value)
```


指示是否在 PivotTable 视图的行轴和列轴上显示数据字段标题和透视字段标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowMemberPropertyTips(boolean value) {#setShowMemberPropertyTips-boolean-}
```
public void setShowMemberPropertyTips(boolean value)
```


指定一个布尔值，指示是否应从 PivotTable 工具提示中省略成员属性信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowPivotStyleColumnHeader(boolean value) {#setShowPivotStyleColumnHeader-boolean-}
```
public void setShowPivotStyleColumnHeader(boolean value)
```


指示是否应对数据透视表中的列标题应用样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowPivotStyleColumnStripes(boolean value) {#setShowPivotStyleColumnStripes-boolean-}
```
public void setShowPivotStyleColumnStripes(boolean value)
```


指示是否对列应用条纹格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowPivotStyleLastColumn(boolean value) {#setShowPivotStyleLastColumn-boolean-}
```
public void setShowPivotStyleLastColumn(boolean value)
```


指示是否已应用列格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowPivotStyleRowHeader(boolean value) {#setShowPivotStyleRowHeader-boolean-}
```
public void setShowPivotStyleRowHeader(boolean value)
```


指示是否应对数据透视表中的行标题应用样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowPivotStyleRowStripes(boolean value) {#setShowPivotStyleRowStripes-boolean-}
```
public void setShowPivotStyleRowStripes(boolean value)
```


指示是否已对行应用条纹格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowRowGrandTotals(boolean value) {#setShowRowGrandTotals-boolean-}
```
public void setShowRowGrandTotals(boolean value)
```


指示是否显示数据透视表行的总计。

**Remarks**

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowRowHeaderCaption(boolean value) {#setShowRowHeaderCaption-boolean-}
```
public void setShowRowHeaderCaption(boolean value)
```


指示是否在 PivotTable 报表中显示行标题标题；指示是否显示字段标题和筛选下拉列表。

**Remarks**

注意：此属性已过时。请改用 PivotTable.ShowHeaders 属性。该方法将在自 2026 年 4 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowValuesRow(boolean value) {#setShowValuesRow-boolean-}
```
public void setShowValuesRow(boolean value)
```


指示是否显示值行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSubtotalHiddenPageItems(boolean value) {#setSubtotalHiddenPageItems-boolean-}
```
public void setSubtotalHiddenPageItems(boolean value)
```


指示在 PivotTable 报表中是否将隐藏的页面字段项包含在行和列小计、区块总计以及总计中。默认值为 False。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTag(String value) {#setTag-java.lang.String-}
```
public void setTag(String value)
```


设置与此 PivotTable 视图关联的用户定义字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn) {#showDetail-int-int-boolean-int-int-}
```
public void showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)
```


在数据区域中显示单个项目的详细信息到新表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | int | 数据区域中第一行数据的偏移量。 |
| columnOffset | int | 数据区域中第一列数据的偏移量。 |
| newSheet | boolean | 在新工作表中显示详细信息。 |
| destRow | int | 目标行。 |
| destColumn | int | 目标列。 |

### showInCompactForm() {#showInCompactForm--}
```
public void showInCompactForm()
```


以紧凑形式布局数据透视表视图。

### showInOutlineForm() {#showInOutlineForm--}
```
public void showInOutlineForm()
```


以大纲形式布局数据透视表。

### showInTabularForm() {#showInTabularForm--}
```
public void showInTabularForm()
```


以表格形式布局数据透视表。

### showReportFilterPage(PivotField pageField) {#showReportFilterPage-com.aspose.cells.PivotField-}
```
public void showReportFilterPage(PivotField pageField)
```


根据 PivotField 显示所有报表筛选页面，PivotField 必须位于 PageFields 中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageField | [PivotField](../../com.aspose.cells/pivotfield) | PivotField 对象 |

### showReportFilterPageByIndex(int posIndex) {#showReportFilterPageByIndex-int-}
```
public void showReportFilterPageByIndex(int posIndex)
```


根据 PageFields 中的位置索引显示所有报表筛选页面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| posIndex | int | PageFields 中的位置索引 |

### showReportFilterPageByName(String fieldName) {#showReportFilterPageByName-java.lang.String-}
```
public void showReportFilterPageByName(String fieldName)
```


根据 PivotField 的名称显示所有报表筛选页面，PivotField 必须位于 PageFields 中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldName | java.lang.String | PivotField 的名称 |

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

