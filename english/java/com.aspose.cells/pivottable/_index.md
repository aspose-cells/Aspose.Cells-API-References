---
title: PivotTable
second_title: Aspose.Cells for Java API Reference
description: Summary description for PivotTable.
type: docs
url: /java/com.aspose.cells/pivottable/
---

**Inheritance:**
java.lang.Object
```
public class PivotTable
```

Summary description for PivotTable.

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
 
         int pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable");
         PivotTable pivot = pivots.get(pivotIndex);
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         int index = pivot.getPivotFilters().add(0, PivotFilterType.COUNT);
         PivotFilter filter = pivot.getPivotFilters().get(index);
         filter.getAutoFilter().filterTop10(0, false, false, 2);
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getPivotFormatConditions().add();
         PivotFormatCondition pfc = pivot.getPivotFormatConditions().get(formatIndex);
         FormatConditionCollection fcc = pfc.getFormatConditions();
         fcc.addArea(pivot.getDataBodyRange());
         int idx = fcc.addCondition(FormatConditionType.CELL_VALUE);
         FormatCondition fc = fcc.get(idx);
         fc.setFormula1("100");
         fc.setOperator(OperatorType.GREATER_OR_EQUAL);
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         PivotTableCalculateOption calculateOption = new PivotTableCalculateOption();
         calculateOption.setRefreshData(true);
         calculateOption.setRefreshCharts(true);
         pivot.calculateData(calculateOption);
 
         //do your business
 
         book.save("out.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [addCalculatedField(String name, String formula)](#addCalculatedField-java.lang.String-java.lang.String-) | Adds a calculated field to pivot field and drag it to data area. |
| [addCalculatedField(String name, String formula, boolean dragToDataArea)](#addCalculatedField-java.lang.String-java.lang.String-boolean-) | Adds a calculated field to pivot field. |
| [addFieldToArea(int fieldType, PivotField pivotField)](#addFieldToArea-int-com.aspose.cells.PivotField-) | Adds the field to the specific area. |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Adds the field to the specific area. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Adds the field to the specific area. |
| [calculateData()](#calculateData--) | Calculates data of pivottable to cells. |
| [calculateData(PivotTableCalculateOption option)](#calculateData-com.aspose.cells.PivotTableCalculateOption-) | Calculates pivot table with options. |
| [calculateRange()](#calculateRange--) | Calculates pivottable's range. |
| [changeDataSource(String[] source)](#changeDataSource-java.lang.String---) | Change data source of the pivottable. |
| [clearData()](#clearData--) | Clear data and formatting of PivotTable view. |
| [copyStyle(PivotTable pivotTable)](#copyStyle-com.aspose.cells.PivotTable-) | Copies named style from another pivot table. |
| [dispose()](#dispose--) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | Gets the specific fields by the field type. |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | Formats selected area of the PivotTable. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | Formats selected area of the PivotTable. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | Formats the cell in the pivottable area |
| [formatAll(Style style)](#formatAll-com.aspose.cells.Style-) | Format all the cell in the pivottable area |
| [formatRow(int row, Style style)](#formatRow-int-com.aspose.cells.Style-) | Format the row data in the pivottable area |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [getAltTextDescription()](#getAltTextDescription--) | Gets the description of the alt text. |
| [getAltTextTitle()](#getAltTextTitle--) | Gets the title of the alter text. |
| [getAutoFormatType()](#getAutoFormatType--) | Gets the auto format type of PivotTable. |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--) | Indicates whether autofitting column width on update |
| [getBaseFields()](#getBaseFields--) | Returns all base pivot fields in the PivotTable. |
| [getButtonArea(int axisType)](#getButtonArea-int-) | Gets the area contains field button. |
| [getCellByDisplayName(String displayName)](#getCellByDisplayName-java.lang.String-) | Gets the [Cell](../../com.aspose.cells/cell) object by the display name of PivotField. |
| [getChildren()](#getChildren--) | Gets the Children Pivot Tables which use this PivotTable data as data source. |
| [getClass()](#getClass--) |  |
| [getColumnFields()](#getColumnFields--) | Returns a PivotFields object that are currently shown as column fields. |
| [getColumnGrand()](#getColumnGrand--) | Indicates whether the PivotTable report shows grand totals for columns. |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--) | Gets the custom Caption of the Column Header of the PivotTable. |
| [getColumnRange()](#getColumnRange--) | Returns a CellArea object that represents the range that contains the column area in the PivotTable report. |
| [getConditionalFormats()](#getConditionalFormats--) | Gets the conditional formats of the pivot table. |
| [getCustomListSort()](#getCustomListSort--) | Indicates whether consider built-in custom list when sort data |
| [getDataBodyRange()](#getDataBodyRange--) | Returns a [CellArea](../../com.aspose.cells/cellarea) object that represents the range that contains the data area in the list between the header row and the insert row. |
| [getDataField()](#getDataField--) | Gets a [PivotField](../../com.aspose.cells/pivotfield) object that represents all the data fields in a PivotTable. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--) | Gets the name of the value area field header in the PivotTable. |
| [getDataFields()](#getDataFields--) | Gets a PivotField object that represents all the data fields in a PivotTable. |
| [getDataSource()](#getDataSource--) | Gets the data source of the pivot table. |
| [getDisplayErrorString()](#getDisplayErrorString--) | Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--) | Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. |
| [getDisplayNullString()](#getDisplayNullString--) | Indicates whether the PivotTable report displays a custom string if the value is null. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--) | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. |
| [getEnableDrilldown()](#getEnableDrilldown--) | Gets whether drilldown is enabled. |
| [getEnableFieldDialog()](#getEnableFieldDialog--) | Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [getEnableFieldList()](#getEnableFieldList--) | Indicates whether the field list for the PivotTable is available on the view of Excel. |
| [getEnableWizard()](#getEnableWizard--) | Indicates whether the PivotTable Wizard is available. |
| [getErrorString()](#getErrorString--) | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--) | Gets the external connection data source. |
| [getFieldListSortAscending()](#getFieldListSortAscending--) | Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [getFields(int fieldType)](#getFields-int-) | Gets the specific pivot field list by the region. |
| [getFilterArea()](#getFilterArea--) | Gets the region of filter region. |
| [getGrandTotalName()](#getGrandTotalName--) | Returns the label that is displayed in the grand total column or row heading. |
| [getHorizontalBreaks()](#getHorizontalBreaks--) | Gets pivot table row index list of horizontal page breaks |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Gets horizontal page breaks of this pivot table. |
| [getIndent()](#getIndent--) | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [getItemPrintTitles()](#getItemPrintTitles--) | Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [getManualUpdate()](#getManualUpdate--) | Indicates whether the PivotTable report is recalculated only at the user's request. |
| [getMergeLabels()](#getMergeLabels--) | True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [getName()](#getName--) | Gets the name of the PivotTable |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--) | Gets the names of external source data connections. |
| [getNullString()](#getNullString--) | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [getPageFieldOrder()](#getPageFieldOrder--) | Gets the order in which page fields are added to the PivotTable report's layout. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--) | Gets the number of page fields in each column or row in the PivotTable report. |
| [getPageFields()](#getPageFields--) | Returns a PivotFields object that are currently shown as page fields. |
| [getPivotFilters()](#getPivotFilters--) | Returns all filters of pivot fields in the pivot table. |
| [getPivotFormatConditions()](#getPivotFormatConditions--) | Gets the Format Conditions of the pivot table. |
| [getPivotFormats()](#getPivotFormats--) | Gets all formats applied to PivotTable. |
| [getPivotTableStyle()](#getPivotTableStyle--) | Gets [TableStyle](../../com.aspose.cells/tablestyle) settings of this pivot table. |
| [getPivotTableStyleName()](#getPivotTableStyleName--) | Gets the pivottable style name. |
| [getPivotTableStyleType()](#getPivotTableStyleType--) | Gets the built-in pivot table style. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [getPrintDrill()](#getPrintDrill--) | Specifies a boolean value that indicates whether drill indicators should be printed. |
| [getPrintTitles()](#getPrintTitles--) | Indicates whether the print titles for the worksheet are set based on the PivotTable report. |
| [getRefreshDataFlag()](#getRefreshDataFlag--) | Indicates whether Refreshing Data or not. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--) | Indicates whether Refresh Data when Opening File. |
| [getRefreshDate()](#getRefreshDate--) | Gets the last date time when the PivotTable was refreshed. |
| [getRefreshedByWho()](#getRefreshedByWho--) | Gets the name of the last user who refreshed this PivotTable |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--) | Indicates whether captions of pivot item on the row area are repeated on each printed page for pivot fields in tabular form. |
| [getRowFields()](#getRowFields--) | Returns a PivotFields object that are currently shown as row fields. |
| [getRowGrand()](#getRowGrand--) | Indicates whether to show grand totals for rows of this pivot table. |
| [getRowHeaderCaption()](#getRowHeaderCaption--) | Gets custom caption of the Row Header in this PivotTable. |
| [getRowRange()](#getRowRange--) | Returns a CellArea object that represents the range that contains the row area in the PivotTable report. |
| [getSaveData()](#getSaveData--) | Indicates whether data for the PivotTable report is saved with the workbook. |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--) | Indicates whether to show grand totals for columns of this pivot table. |
| [getShowDataTips()](#getShowDataTips--) | Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [getShowDrill()](#getShowDrill--) | Gets whether showing expand/collapse buttons. |
| [getShowEmptyCol()](#getShowEmptyCol--) | Indicates whether to include empty columns in the table |
| [getShowEmptyRow()](#getShowEmptyRow--) | Indicates whether to include empty rows in the table. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--) | Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--) | Indicates whether the column header in the pivot table should have the style applied. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--) | Indicates whether stripe formatting is applied for column. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--) | Indicates whether the column formatting is applied. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--) | Indicates whether the row header in the pivot table should have the style applied. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--) | Indicates whether row stripe formatting is applied. |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--) | Indicates whether to show grand totals for rows of the pivot table. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--) | Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs |
| [getShowValuesRow()](#getShowValuesRow--) | Indicates whether showing values row. |
| [getSource()](#getSource--) | Get the data source of this pivottable. |
| [getSource(boolean isOriginal)](#getSource-boolean-) | Get the data source of this pivottable. |
| [getSourceDataConnections()](#getSourceDataConnections--) | Gets the external connection data sources. |
| [getSourceType()](#getSourceType--) | Gets the data source type of the pivot table. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--) | Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. |
| [getTableRange1()](#getTableRange1--) | Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. |
| [getTableRange2()](#getTableRange2--) | Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. |
| [getTag()](#getTag--) | Gets a user-defined string that is associated with this PivotTable view. |
| [getTopRightArea()](#getTopRightArea--) | Represents the blank area at the top-right of the PivotTable (top-left for RTL sheets). |
| [getValuesField()](#getValuesField--) | Gets a [PivotField](../../com.aspose.cells/pivotfield) object that represents all the data fields in a PivotTable. |
| [hasBlankRows()](#hasBlankRows--) | Indicates whether to add blank rows. |
| [hashCode()](#hashCode--) |  |
| [isAutoFormat()](#isAutoFormat--) | Indicates whether the PivotTable report is automatically formatted. |
| [isExcel2003Compatible()](#isExcel2003Compatible--) | Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. |
| [isGridDropZones()](#isGridDropZones--) | Indicates whether the PivotTable report displays classic pivottable layout. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [isSelected()](#isSelected--) | Indicates whether this PivotTable is selected. |
| [move(int row, int column)](#move-int-int-) | Moves the PivotTable to a different location in the worksheet. |
| [move(String destCellName)](#move-java.lang.String-) | Moves the PivotTable to a different location in the worksheet. |
| [moveTo(int row, int column)](#moveTo-int-int-) | Moves the PivotTable to a different location in the worksheet. |
| [moveTo(String destCellName)](#moveTo-java.lang.String-) | Moves the PivotTable to a different location in the worksheet. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | Refreshes pivottable's data and setting from it's data source. |
| [refreshData(PivotTableRefreshOption option)](#refreshData-com.aspose.cells.PivotTableRefreshOption-) | Refreshes pivottable's data and setting from it's data source with options. |
| [removeField(int fieldType, PivotField pivotField)](#removeField-int-com.aspose.cells.PivotField-) | Remove field from specific field area |
| [removeField(int fieldType, int baseFieldIndex)](#removeField-int-int-) | Removes a field from specific field area |
| [removeField(int fieldType, String fieldName)](#removeField-int-java.lang.String-) | Removes a field from specific field area |
| [selectArea(CellArea ca)](#selectArea-com.aspose.cells.CellArea-) | Select an area of pivot table view. |
| [setAllowMultipleFiltersPerField(boolean value)](#setAllowMultipleFiltersPerField-boolean-) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [setAltTextDescription(String value)](#setAltTextDescription-java.lang.String-) | Gets the description of the alt text. |
| [setAltTextTitle(String value)](#setAltTextTitle-java.lang.String-) | Sets the title of the alter text. |
| [setAutoFormat(boolean value)](#setAutoFormat-boolean-) | Indicates whether the PivotTable report is automatically formatted. |
| [setAutoFormatType(int value)](#setAutoFormatType-int-) | Sets the auto format type of PivotTable. |
| [setAutoGroupField(PivotField pivotField)](#setAutoGroupField-com.aspose.cells.PivotField-) | Sets auto field group by the PivotTable. |
| [setAutoGroupField(int baseFieldIndex)](#setAutoGroupField-int-) | Sets auto field group by the PivotTable. |
| [setAutofitColumnWidthOnUpdate(boolean value)](#setAutofitColumnWidthOnUpdate-boolean-) | Indicates whether autofitting column width on update |
| [setColumnGrand(boolean value)](#setColumnGrand-boolean-) | Indicates whether the PivotTable report shows grand totals for columns. |
| [setColumnHeaderCaption(String value)](#setColumnHeaderCaption-java.lang.String-) | Sets the custom Caption of the Column Header of the PivotTable. |
| [setCustomListSort(boolean value)](#setCustomListSort-boolean-) | Indicates whether consider built-in custom list when sort data |
| [setDataFieldHeaderName(String value)](#setDataFieldHeaderName-java.lang.String-) | Sets the name of the value area field header in the PivotTable. |
| [setDataSource(String[] value)](#setDataSource-java.lang.String---) | Sets the data source of the pivot table. |
| [setDisplayErrorString(boolean value)](#setDisplayErrorString-boolean-) | Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [setDisplayImmediateItems(boolean value)](#setDisplayImmediateItems-boolean-) | Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. |
| [setDisplayNullString(boolean value)](#setDisplayNullString-boolean-) | Indicates whether the PivotTable report displays a custom string if the value is null. |
| [setEnableDataValueEditing(boolean value)](#setEnableDataValueEditing-boolean-) | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. |
| [setEnableDrilldown(boolean value)](#setEnableDrilldown-boolean-) | Gets whether drilldown is enabled. |
| [setEnableFieldDialog(boolean value)](#setEnableFieldDialog-boolean-) | Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [setEnableFieldList(boolean value)](#setEnableFieldList-boolean-) | Indicates whether the field list for the PivotTable is available on the view of Excel. |
| [setEnableWizard(boolean value)](#setEnableWizard-boolean-) | Indicates whether the PivotTable Wizard is available. |
| [setErrorString(String value)](#setErrorString-java.lang.String-) | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [setExcel2003Compatible(boolean value)](#setExcel2003Compatible-boolean-) | Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. |
| [setFieldListSortAscending(boolean value)](#setFieldListSortAscending-boolean-) | Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [setGrandTotalName(String value)](#setGrandTotalName-java.lang.String-) | Returns the label that is displayed in the grand total column or row heading. |
| [setGridDropZones(boolean value)](#setGridDropZones-boolean-) | Indicates whether the PivotTable report displays classic pivottable layout. |
| [setHasBlankRows(boolean value)](#setHasBlankRows-boolean-) | Indicates whether to add blank rows. |
| [setIndent(int value)](#setIndent-int-) | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [setItemPrintTitles(boolean value)](#setItemPrintTitles-boolean-) | Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [setManualGroupField(PivotField pivotField, DateTime startVal, DateTime endVal, ArrayList groupByList, int intervalNum)](#setManualGroupField-com.aspose.cells.PivotField-com.aspose.cells.DateTime-com.aspose.cells.DateTime-java.util.ArrayList-int-) | Sets manual field group by the PivotTable. |
| [setManualGroupField(PivotField pivotField, double startVal, double endVal, ArrayList groupByList, double intervalNum)](#setManualGroupField-com.aspose.cells.PivotField-double-double-java.util.ArrayList-double-) | Sets manual field group by the PivotTable. |
| [setManualGroupField(int baseFieldIndex, DateTime startVal, DateTime endVal, ArrayList groupByList, int intervalNum)](#setManualGroupField-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-java.util.ArrayList-int-) | Sets manual field group by the PivotTable. |
| [setManualGroupField(int baseFieldIndex, double startVal, double endVal, ArrayList groupByList, double intervalNum)](#setManualGroupField-int-double-double-java.util.ArrayList-double-) | Sets manual field group by the PivotTable. |
| [setManualUpdate(boolean value)](#setManualUpdate-boolean-) | Indicates whether the PivotTable report is recalculated only at the user's request. |
| [setMergeLabels(boolean value)](#setMergeLabels-boolean-) | True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [setMultipleFieldFilters(boolean value)](#setMultipleFieldFilters-boolean-) | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [setName(String value)](#setName-java.lang.String-) | Gets the name of the PivotTable |
| [setNullString(String value)](#setNullString-java.lang.String-) | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [setPageFieldOrder(int value)](#setPageFieldOrder-int-) | Sets the order in which page fields are added to the PivotTable report's layout. |
| [setPageFieldWrapCount(int value)](#setPageFieldWrapCount-int-) | Gets the number of page fields in each column or row in the PivotTable report. |
| [setPivotTableStyle(TableStyle value)](#setPivotTableStyle-com.aspose.cells.TableStyle-) | Gets [TableStyle](../../com.aspose.cells/tablestyle) settings of this pivot table. |
| [setPivotTableStyleName(String value)](#setPivotTableStyleName-java.lang.String-) | Sets the pivottable style name. |
| [setPivotTableStyleType(int value)](#setPivotTableStyleType-int-) | Sets the built-in pivot table style. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [setPrintDrill(boolean value)](#setPrintDrill-boolean-) | Specifies a boolean value that indicates whether drill indicators should be printed. |
| [setPrintTitles(boolean value)](#setPrintTitles-boolean-) | Indicates whether the print titles for the worksheet are set based on the PivotTable report. |
| [setRefreshDataFlag(boolean value)](#setRefreshDataFlag-boolean-) | Indicates whether Refreshing Data or not. |
| [setRefreshDataOnOpeningFile(boolean value)](#setRefreshDataOnOpeningFile-boolean-) | Indicates whether Refresh Data when Opening File. |
| [setRepeatItemsOnEachPrintedPage(boolean value)](#setRepeatItemsOnEachPrintedPage-boolean-) | Indicates whether captions of pivot item on the row area are repeated on each printed page for pivot fields in tabular form. |
| [setRowGrand(boolean value)](#setRowGrand-boolean-) | Indicates whether to show grand totals for rows of this pivot table. |
| [setRowHeaderCaption(String value)](#setRowHeaderCaption-java.lang.String-) | Sets custom caption of the Row Header in this PivotTable. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Indicates whether data for the PivotTable report is saved with the workbook. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indicates whether this PivotTable is selected. |
| [setShowColumnGrandTotals(boolean value)](#setShowColumnGrandTotals-boolean-) | Indicates whether to show grand totals for columns of this pivot table. |
| [setShowDataTips(boolean value)](#setShowDataTips-boolean-) | Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [setShowDrill(boolean value)](#setShowDrill-boolean-) | Sets whether showing expand/collapse buttons. |
| [setShowEmptyCol(boolean value)](#setShowEmptyCol-boolean-) | Indicates whether to include empty columns in the table |
| [setShowEmptyRow(boolean value)](#setShowEmptyRow-boolean-) | Indicates whether to include empty rows in the table. |
| [setShowMemberPropertyTips(boolean value)](#setShowMemberPropertyTips-boolean-) | Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [setShowPivotStyleColumnHeader(boolean value)](#setShowPivotStyleColumnHeader-boolean-) | Indicates whether the column header in the pivot table should have the style applied. |
| [setShowPivotStyleColumnStripes(boolean value)](#setShowPivotStyleColumnStripes-boolean-) | Indicates whether stripe formatting is applied for column. |
| [setShowPivotStyleLastColumn(boolean value)](#setShowPivotStyleLastColumn-boolean-) | Indicates whether the column formatting is applied. |
| [setShowPivotStyleRowHeader(boolean value)](#setShowPivotStyleRowHeader-boolean-) | Indicates whether the row header in the pivot table should have the style applied. |
| [setShowPivotStyleRowStripes(boolean value)](#setShowPivotStyleRowStripes-boolean-) | Indicates whether row stripe formatting is applied. |
| [setShowRowGrandTotals(boolean value)](#setShowRowGrandTotals-boolean-) | Indicates whether to show grand totals for rows of the pivot table. |
| [setShowRowHeaderCaption(boolean value)](#setShowRowHeaderCaption-boolean-) | Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs |
| [setShowValuesRow(boolean value)](#setShowValuesRow-boolean-) | Indicates whether showing values row. |
| [setSubtotalHiddenPageItems(boolean value)](#setSubtotalHiddenPageItems-boolean-) | Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. |
| [setTag(String value)](#setTag-java.lang.String-) | Sets a user-defined string that is associated with this PivotTable view. |
| [setUngroup(PivotField pivotField)](#setUngroup-com.aspose.cells.PivotField-) | Sets ungroup by the PivotTable |
| [setUngroup(int baseFieldIndex)](#setUngroup-int-) | Sets ungroup by the PivotTable |
| [showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)](#showDetail-int-int-boolean-int-int-) | Show the detail of one item in the data region to a new Table. |
| [showInCompactForm()](#showInCompactForm--) | Layouts the PivotTable view in compact form. |
| [showInOutlineForm()](#showInOutlineForm--) | Layouts the PivotTable in outline form. |
| [showInTabularForm()](#showInTabularForm--) | Layouts the PivotTable in tabular form. |
| [showReportFilterPage(PivotField pageField)](#showReportFilterPage-com.aspose.cells.PivotField-) | Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields. |
| [showReportFilterPageByIndex(int posIndex)](#showReportFilterPageByIndex-int-) | Show all the report filter pages according to the position index in the PageFields |
| [showReportFilterPageByName(String fieldName)](#showReportFilterPageByName-java.lang.String-) | Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedField(String name, String formula) {#addCalculatedField-java.lang.String-java.lang.String-}
```
public void addCalculatedField(String name, String formula)
```


Adds a calculated field to pivot field and drag it to data area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the calculated field |
| formula | java.lang.String | The formula of the calculated field. |

### addCalculatedField(String name, String formula, boolean dragToDataArea) {#addCalculatedField-java.lang.String-java.lang.String-boolean-}
```
public void addCalculatedField(String name, String formula, boolean dragToDataArea)
```


Adds a calculated field to pivot field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the calculated field |
| formula | java.lang.String | The formula of the calculated field. |
| dragToDataArea | boolean | True,drag this field to data area immediately |

### addFieldToArea(int fieldType, PivotField pivotField) {#addFieldToArea-int-com.aspose.cells.PivotField-}
```
public int addFieldToArea(int fieldType, PivotField pivotField)
```


Adds the field to the specific area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). the fields area type. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | the field in the base fields. |

**Returns:**
int - the field position in the specific fields.
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Adds the field to the specific area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The fields area type. |
| baseFieldIndex | int | The field index in the base fields. |

**Returns:**
int - The field position in the specific fields.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Adds the field to the specific area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The fields area type. |
| fieldName | java.lang.String | The name in the base fields. |

**Returns:**
int - The field position in the specific fields.If there is no field named as it, return -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Calculates data of pivottable to cells.

**Remarks**

Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.

### calculateData(PivotTableCalculateOption option) {#calculateData-com.aspose.cells.PivotTableCalculateOption-}
```
public void calculateData(PivotTableCalculateOption option)
```


Calculates pivot table with options.

**Remarks**

If PivotTableCalculateOption.RefreshData is true, this method will refresh pivot cache from data source,then calculate all pivot tables based same pivot cache.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../../com.aspose.cells/pivottablecalculateoption) | The options for calculating the pivot table |

### calculateRange() {#calculateRange--}
```
public void calculateRange()
```


Calculates pivottable's range.

**Remarks**

If this method is not been called,maybe the pivottable range is not corrected.

### changeDataSource(String[] source) {#changeDataSource-java.lang.String---}
```
public void changeDataSource(String[] source)
```


Change data source of the pivottable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.lang.String[] |  |

### clearData() {#clearData--}
```
public void clearData()
```


Clear data and formatting of PivotTable view.

**Remarks**

If this method is not called before you add or delete PivotField, Maybe the PivotTable data is not corrected

### copyStyle(PivotTable pivotTable) {#copyStyle-com.aspose.cells.PivotTable-}
```
public void copyStyle(PivotTable pivotTable)
```


Copies named style from another pivot table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Source pivot table. |

### dispose() {#dispose--}
```
public void dispose()
```


Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

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
### fields(int fieldType) {#fields-int-}
```
public PivotFieldCollection fields(int fieldType)
```


Gets the specific fields by the field type.

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GetFields(PivotFieldType) method. This method will be removed 12 months later since May 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). the field type. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific field collection
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


Formats selected area of the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | The range of the cells. |
| style | [Style](../../com.aspose.cells/style) | The style |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


Formats selected area of the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | The selected pivot view area. |
| style | [Style](../../com.aspose.cells/style) | The formatted setting. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


Formats the cell in the pivottable area

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row Index of the cell |
| column | int | Column index of the cell |
| style | [Style](../../com.aspose.cells/style) | Style which is to format the cell |

### formatAll(Style style) {#formatAll-com.aspose.cells.Style-}
```
public void formatAll(Style style)
```


Format all the cell in the pivottable area

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Style which is to format |

### formatRow(int row, Style style) {#formatRow-int-com.aspose.cells.Style-}
```
public void formatRow(int row, Style style)
```


Format the row data in the pivottable area

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row Index of the Row object |
| style | [Style](../../com.aspose.cells/style) | Style which is to format |

### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```
public boolean getAllowMultipleFiltersPerField()
```


Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

**Returns:**
boolean
### getAltTextDescription() {#getAltTextDescription--}
```
public String getAltTextDescription()
```


Gets the description of the alt text.

**Returns:**
java.lang.String
### getAltTextTitle() {#getAltTextTitle--}
```
public String getAltTextTitle()
```


Gets the title of the alter text.

**Returns:**
java.lang.String
### getAutoFormatType() {#getAutoFormatType--}
```
public int getAutoFormatType()
```


Gets the auto format type of PivotTable.

See [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Returns:**
int
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```
public boolean getAutofitColumnWidthOnUpdate()
```


Indicates whether autofitting column width on update

**Returns:**
boolean
### getBaseFields() {#getBaseFields--}
```
public PivotFieldCollection getBaseFields()
```


Returns all base pivot fields in the PivotTable.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getButtonArea(int axisType) {#getButtonArea-int-}
```
public CellArea getButtonArea(int axisType)
```


Gets the area contains field button.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The region type. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - 
### getCellByDisplayName(String displayName) {#getCellByDisplayName-java.lang.String-}
```
public Cell getCellByDisplayName(String displayName)
```


Gets the [Cell](../../com.aspose.cells/cell) object by the display name of PivotField.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| displayName | java.lang.String | the DisplayName of PivotField |

**Returns:**
[Cell](../../com.aspose.cells/cell) - the Cell object
### getChildren() {#getChildren--}
```
public PivotTable[] getChildren()
```


Gets the Children Pivot Tables which use this PivotTable data as data source.

**Returns:**
com.aspose.cells.PivotTable[] - the PivotTable array object
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


Returns a PivotFields object that are currently shown as column fields.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getColumnGrand() {#getColumnGrand--}
```
public boolean getColumnGrand()
```


Indicates whether the PivotTable report shows grand totals for columns.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.ShowColumnGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```
public String getColumnHeaderCaption()
```


Gets the custom Caption of the Column Header of the PivotTable.

**Returns:**
java.lang.String
### getColumnRange() {#getColumnRange--}
```
public CellArea getColumnRange()
```


Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getConditionalFormats() {#getConditionalFormats--}
```
public PivotConditionalFormatCollection getConditionalFormats()
```


Gets the conditional formats of the pivot table.

**Returns:**
[PivotConditionalFormatCollection](../../com.aspose.cells/pivotconditionalformatcollection)
### getCustomListSort() {#getCustomListSort--}
```
public boolean getCustomListSort()
```


Indicates whether consider built-in custom list when sort data

**Returns:**
boolean
### getDataBodyRange() {#getDataBodyRange--}
```
public CellArea getDataBodyRange()
```


Returns a [CellArea](../../com.aspose.cells/cellarea) object that represents the range that contains the data area in the list between the header row and the insert row. Read-only.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getDataField() {#getDataField--}
```
public PivotField getDataField()
```


Gets a [PivotField](../../com.aspose.cells/pivotfield) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotTable.ValuesField property. This method will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```
public String getDataFieldHeaderName()
```


Gets the name of the value area field header in the PivotTable.

**Returns:**
java.lang.String
### getDataFields() {#getDataFields--}
```
public PivotFieldCollection getDataFields()
```


Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getDataSource() {#getDataSource--}
```
public String[] getDataSource()
```


Gets the data source of the pivot table.

**Returns:**
java.lang.String[]
### getDisplayErrorString() {#getDisplayErrorString--}
```
public boolean getDisplayErrorString()
```


Indicates whether the PivotTable report displays a custom string in cells that contain errors.

**Returns:**
boolean
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```
public boolean getDisplayImmediateItems()
```


Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true.

**Returns:**
boolean
### getDisplayNullString() {#getDisplayNullString--}
```
public boolean getDisplayNullString()
```


Indicates whether the PivotTable report displays a custom string if the value is null.

**Returns:**
boolean
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```
public boolean getEnableDataValueEditing()
```


Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area

**Returns:**
boolean
### getEnableDrilldown() {#getEnableDrilldown--}
```
public boolean getEnableDrilldown()
```


Gets whether drilldown is enabled.

**Returns:**
boolean
### getEnableFieldDialog() {#getEnableFieldDialog--}
```
public boolean getEnableFieldDialog()
```


Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field.

**Returns:**
boolean
### getEnableFieldList() {#getEnableFieldList--}
```
public boolean getEnableFieldList()
```


Indicates whether the field list for the PivotTable is available on the view of Excel.

**Returns:**
boolean
### getEnableWizard() {#getEnableWizard--}
```
public boolean getEnableWizard()
```


Indicates whether the PivotTable Wizard is available.

**Returns:**
boolean
### getErrorString() {#getErrorString--}
```
public String getErrorString()
```


Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string.

**Returns:**
java.lang.String
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```
public ExternalConnection getExternalConnectionDataSource()
```


Gets the external connection data source.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.GetSourceDataConnections() method. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getFieldListSortAscending() {#getFieldListSortAscending--}
```
public boolean getFieldListSortAscending()
```


Indicates whether fields in the PivotTable are sorted in non-default order in the field list.

**Returns:**
boolean
### getFields(int fieldType) {#getFields-int-}
```
public PivotFieldCollection getFields(int fieldType)
```


Gets the specific pivot field list by the region.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). the region type. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific pivot field collection
### getFilterArea() {#getFilterArea--}
```
public CellArea getFilterArea()
```


Gets the region of filter region.

**Remarks**

Only valid if filter pivot fields exists.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getGrandTotalName() {#getGrandTotalName--}
```
public String getGrandTotalName()
```


Returns the label that is displayed in the grand total column or row heading. The default value is the string "Grand Total".

**Returns:**
java.lang.String
### getHorizontalBreaks() {#getHorizontalBreaks--}
```
public ArrayList getHorizontalBreaks()
```


Gets pivot table row index list of horizontal page breaks

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotTable.GetHorizontalPageBreaks() method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.util.ArrayList - 
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public int[] getHorizontalPageBreaks()
```


Gets horizontal page breaks of this pivot table.

**Returns:**
int[] - 
### getIndent() {#getIndent--}
```
public int getIndent()
```


Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.

**Returns:**
int
### getItemPrintTitles() {#getItemPrintTitles--}
```
public boolean getItemPrintTitles()
```


Indicates whether PivotItem names should be repeated at the top of each printed page.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.RepeatItemsOnEachPrintedPage property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getManualUpdate() {#getManualUpdate--}
```
public boolean getManualUpdate()
```


Indicates whether the PivotTable report is recalculated only at the user's request.

**Returns:**
boolean
### getMergeLabels() {#getMergeLabels--}
```
public boolean getMergeLabels()
```


True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells.

**Returns:**
boolean
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

See [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Gets the name of the PivotTable

**Returns:**
java.lang.String
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
```
public String[] getNamesOfSourceDataConnections()
```


Gets the names of external source data connections.

**Returns:**
java.lang.String[]
### getNullString() {#getNullString--}
```
public String getNullString()
```


Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string.

**Returns:**
java.lang.String
### getPageFieldOrder() {#getPageFieldOrder--}
```
public int getPageFieldOrder()
```


Gets the order in which page fields are added to the PivotTable report's layout.

See [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```
public int getPageFieldWrapCount()
```


Gets the number of page fields in each column or row in the PivotTable report.

**Returns:**
int
### getPageFields() {#getPageFields--}
```
public PivotFieldCollection getPageFields()
```


Returns a PivotFields object that are currently shown as page fields.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getPivotFilters() {#getPivotFilters--}
```
public PivotFilterCollection getPivotFilters()
```


Returns all filters of pivot fields in the pivot table.

**Returns:**
[PivotFilterCollection](../../com.aspose.cells/pivotfiltercollection)
### getPivotFormatConditions() {#getPivotFormatConditions--}
```
public PivotFormatConditionCollection getPivotFormatConditions()
```


Gets the Format Conditions of the pivot table.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.ConditionalFormats property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[PivotFormatConditionCollection](../../com.aspose.cells/pivotformatconditioncollection)
### getPivotFormats() {#getPivotFormats--}
```
public PivotTableFormatCollection getPivotFormats()
```


Gets all formats applied to PivotTable.

**Returns:**
[PivotTableFormatCollection](../../com.aspose.cells/pivottableformatcollection)
### getPivotTableStyle() {#getPivotTableStyle--}
```
public TableStyle getPivotTableStyle()
```


Gets [TableStyle](../../com.aspose.cells/tablestyle) settings of this pivot table.

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle)
### getPivotTableStyleName() {#getPivotTableStyleName--}
```
public String getPivotTableStyleName()
```


Gets the pivottable style name.

**Returns:**
java.lang.String
### getPivotTableStyleType() {#getPivotTableStyleType--}
```
public int getPivotTableStyleType()
```


Gets the built-in pivot table style.

See [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Returns:**
int
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated.

**Returns:**
boolean
### getPrintDrill() {#getPrintDrill--}
```
public boolean getPrintDrill()
```


Specifies a boolean value that indicates whether drill indicators should be printed. Print expand/collapse buttons when displayed on pivottable.

**Returns:**
boolean
### getPrintTitles() {#getPrintTitles--}
```
public boolean getPrintTitles()
```


Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false.

**Returns:**
boolean
### getRefreshDataFlag() {#getRefreshDataFlag--}
```
public boolean getRefreshDataFlag()
```


Indicates whether Refreshing Data or not.

**Remarks**

NOTE: This method is now obsolete. Instead, This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```
public boolean getRefreshDataOnOpeningFile()
```


Indicates whether Refresh Data when Opening File.

**Returns:**
boolean
### getRefreshDate() {#getRefreshDate--}
```
public DateTime getRefreshDate()
```


Gets the last date time when the PivotTable was refreshed.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getRefreshedByWho() {#getRefreshedByWho--}
```
public String getRefreshedByWho()
```


Gets the name of the last user who refreshed this PivotTable

**Returns:**
java.lang.String
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```
public boolean getRepeatItemsOnEachPrintedPage()
```


Indicates whether captions of pivot item on the row area are repeated on each printed page for pivot fields in tabular form.

**Returns:**
boolean
### getRowFields() {#getRowFields--}
```
public PivotFieldCollection getRowFields()
```


Returns a PivotFields object that are currently shown as row fields.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getRowGrand() {#getRowGrand--}
```
public boolean getRowGrand()
```


Indicates whether to show grand totals for rows of this pivot table.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.ShowRowGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getRowHeaderCaption() {#getRowHeaderCaption--}
```
public String getRowHeaderCaption()
```


Gets custom caption of the Row Header in this PivotTable.

**Returns:**
java.lang.String
### getRowRange() {#getRowRange--}
```
public CellArea getRowRange()
```


Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Indicates whether data for the PivotTable report is saved with the workbook.

**Returns:**
boolean
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```
public boolean getShowColumnGrandTotals()
```


Indicates whether to show grand totals for columns of this pivot table.

**Returns:**
boolean
### getShowDataTips() {#getShowDataTips--}
```
public boolean getShowDataTips()
```


Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells.

**Returns:**
boolean
### getShowDrill() {#getShowDrill--}
```
public boolean getShowDrill()
```


Gets whether showing expand/collapse buttons.

**Returns:**
boolean
### getShowEmptyCol() {#getShowEmptyCol--}
```
public boolean getShowEmptyCol()
```


Indicates whether to include empty columns in the table

**Returns:**
boolean
### getShowEmptyRow() {#getShowEmptyRow--}
```
public boolean getShowEmptyRow()
```


Indicates whether to include empty rows in the table.

**Returns:**
boolean
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```
public boolean getShowMemberPropertyTips()
```


Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips.

**Returns:**
boolean
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```
public boolean getShowPivotStyleColumnHeader()
```


Indicates whether the column header in the pivot table should have the style applied.

**Returns:**
boolean
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```
public boolean getShowPivotStyleColumnStripes()
```


Indicates whether stripe formatting is applied for column.

**Returns:**
boolean
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```
public boolean getShowPivotStyleLastColumn()
```


Indicates whether the column formatting is applied.

**Returns:**
boolean
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```
public boolean getShowPivotStyleRowHeader()
```


Indicates whether the row header in the pivot table should have the style applied.

**Returns:**
boolean
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```
public boolean getShowPivotStyleRowStripes()
```


Indicates whether row stripe formatting is applied.

**Returns:**
boolean
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```
public boolean getShowRowGrandTotals()
```


Indicates whether to show grand totals for rows of the pivot table.

**Remarks**

**Returns:**
boolean
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```
public boolean getShowRowHeaderCaption()
```


Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs

**Returns:**
boolean
### getShowValuesRow() {#getShowValuesRow--}
```
public boolean getShowValuesRow()
```


Indicates whether showing values row.

**Returns:**
boolean
### getSource() {#getSource--}
```
public String[] getSource()
```


Get the data source of this pivottable.

**Returns:**
java.lang.String[]
### getSource(boolean isOriginal) {#getSource-boolean-}
```
public String[] getSource(boolean isOriginal)
```


Get the data source of this pivottable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isOriginal | boolean | Indicates whether to return original or display data source. |

**Returns:**
java.lang.String[] - 
### getSourceDataConnections() {#getSourceDataConnections--}
```
public ExternalConnection[] getSourceDataConnections()
```


Gets the external connection data sources.

**Returns:**
com.aspose.cells.ExternalConnection[]
### getSourceType() {#getSourceType--}
```
public byte getSourceType()
```


Gets the data source type of the pivot table.

See [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```
public boolean getSubtotalHiddenPageItems()
```


Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False.

**Returns:**
boolean
### getTableRange1() {#getTableRange1--}
```
public CellArea getTableRange1()
```


Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTableRange2() {#getTableRange2--}
```
public CellArea getTableRange2()
```


Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTag() {#getTag--}
```
public String getTag()
```


Gets a user-defined string that is associated with this PivotTable view.

**Returns:**
java.lang.String
### getTopRightArea() {#getTopRightArea--}
```
public CellArea getTopRightArea()
```


Represents the blank area at the top-right of the PivotTable (top-left for RTL sheets).

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getValuesField() {#getValuesField--}
```
public PivotField getValuesField()
```


Gets a [PivotField](../../com.aspose.cells/pivotfield) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### hasBlankRows() {#hasBlankRows--}
```
public boolean hasBlankRows()
```


Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.

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


Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003

**Returns:**
boolean
### isExcel2003Compatible() {#isExcel2003Compatible--}
```
public boolean isExcel2003Compatible()
```


Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true.

**Returns:**
boolean
### isGridDropZones() {#isGridDropZones--}
```
public boolean isGridDropZones()
```


Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)

**Returns:**
boolean
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```
public boolean isMultipleFieldFilters()
```


Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.AllowMultipleFiltersPerField property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Indicates whether this PivotTable is selected.

**Returns:**
boolean
### move(int row, int column) {#move-int-int-}
```
public void move(int row, int column)
```


Moves the PivotTable to a different location in the worksheet.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.MoveTo() method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | row index. |
| column | int | column index. |

### move(String destCellName) {#move-java.lang.String-}
```
public void move(String destCellName)
```


Moves the PivotTable to a different location in the worksheet.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.MoveTo() method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destCellName | java.lang.String | the dest cell name. |

### moveTo(int row, int column) {#moveTo-int-int-}
```
public void moveTo(int row, int column)
```


Moves the PivotTable to a different location in the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | row index. |
| column | int | column index. |

### moveTo(String destCellName) {#moveTo-java.lang.String-}
```
public void moveTo(String destCellName)
```


Moves the PivotTable to a different location in the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destCellName | java.lang.String | the dest cell name. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshData() {#refreshData--}
```
public int refreshData()
```


Refreshes pivottable's data and setting from it's data source.

**Remarks**

We will gather data from data source to a pivot cache ,then calculate the data in the cache to the cells. This method is only used to gather all data to a pivot cache.

**Returns:**
int
### refreshData(PivotTableRefreshOption option) {#refreshData-com.aspose.cells.PivotTableRefreshOption-}
```
public int refreshData(PivotTableRefreshOption option)
```


Refreshes pivottable's data and setting from it's data source with options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | The options for refreshing data source of pivot table. |

**Returns:**
int
### removeField(int fieldType, PivotField pivotField) {#removeField-int-com.aspose.cells.PivotField-}
```
public void removeField(int fieldType, PivotField pivotField)
```


Remove field from specific field area

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). the fields area type. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | the field in the base fields. |

### removeField(int fieldType, int baseFieldIndex) {#removeField-int-int-}
```
public void removeField(int fieldType, int baseFieldIndex)
```


Removes a field from specific field area

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The fields area type. |
| baseFieldIndex | int | The field index in the base fields. |

### removeField(int fieldType, String fieldName) {#removeField-int-java.lang.String-}
```
public void removeField(int fieldType, String fieldName)
```


Removes a field from specific field area

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The fields area type. |
| fieldName | java.lang.String | The name in the base fields. |

### selectArea(CellArea ca) {#selectArea-com.aspose.cells.CellArea-}
```
public PivotAreaCollection selectArea(CellArea ca)
```


Select an area of pivot table view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | The cell area. |

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection) - 
### setAllowMultipleFiltersPerField(boolean value) {#setAllowMultipleFiltersPerField-boolean-}
```
public void setAllowMultipleFiltersPerField(boolean value)
```


Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAltTextDescription(String value) {#setAltTextDescription-java.lang.String-}
```
public void setAltTextDescription(String value)
```


Gets the description of the alt text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAltTextTitle(String value) {#setAltTextTitle-java.lang.String-}
```
public void setAltTextTitle(String value)
```


Sets the title of the alter text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAutoFormat(boolean value) {#setAutoFormat-boolean-}
```
public void setAutoFormat(boolean value)
```


Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoFormatType(int value) {#setAutoFormatType-int-}
```
public void setAutoFormatType(int value)
```


Sets the auto format type of PivotTable.

See [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoGroupField(PivotField pivotField) {#setAutoGroupField-com.aspose.cells.PivotField-}
```
public void setAutoGroupField(PivotField pivotField)
```


Sets auto field group by the PivotTable.

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | The row or column field in the specific fields |

### setAutoGroupField(int baseFieldIndex) {#setAutoGroupField-int-}
```
public void setAutoGroupField(int baseFieldIndex)
```


Sets auto field group by the PivotTable.

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The row or column field index in the base fields |

### setAutofitColumnWidthOnUpdate(boolean value) {#setAutofitColumnWidthOnUpdate-boolean-}
```
public void setAutofitColumnWidthOnUpdate(boolean value)
```


Indicates whether autofitting column width on update

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setColumnGrand(boolean value) {#setColumnGrand-boolean-}
```
public void setColumnGrand(boolean value)
```


Indicates whether the PivotTable report shows grand totals for columns.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.ShowColumnGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setColumnHeaderCaption(String value) {#setColumnHeaderCaption-java.lang.String-}
```
public void setColumnHeaderCaption(String value)
```


Sets the custom Caption of the Column Header of the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCustomListSort(boolean value) {#setCustomListSort-boolean-}
```
public void setCustomListSort(boolean value)
```


Indicates whether consider built-in custom list when sort data

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDataFieldHeaderName(String value) {#setDataFieldHeaderName-java.lang.String-}
```
public void setDataFieldHeaderName(String value)
```


Sets the name of the value area field header in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDataSource(String[] value) {#setDataSource-java.lang.String---}
```
public void setDataSource(String[] value)
```


Sets the data source of the pivot table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String[] |  |

### setDisplayErrorString(boolean value) {#setDisplayErrorString-boolean-}
```
public void setDisplayErrorString(boolean value)
```


Indicates whether the PivotTable report displays a custom string in cells that contain errors.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDisplayImmediateItems(boolean value) {#setDisplayImmediateItems-boolean-}
```
public void setDisplayImmediateItems(boolean value)
```


Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDisplayNullString(boolean value) {#setDisplayNullString-boolean-}
```
public void setDisplayNullString(boolean value)
```


Indicates whether the PivotTable report displays a custom string if the value is null.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableDataValueEditing(boolean value) {#setEnableDataValueEditing-boolean-}
```
public void setEnableDataValueEditing(boolean value)
```


Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableDrilldown(boolean value) {#setEnableDrilldown-boolean-}
```
public void setEnableDrilldown(boolean value)
```


Gets whether drilldown is enabled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableFieldDialog(boolean value) {#setEnableFieldDialog-boolean-}
```
public void setEnableFieldDialog(boolean value)
```


Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableFieldList(boolean value) {#setEnableFieldList-boolean-}
```
public void setEnableFieldList(boolean value)
```


Indicates whether the field list for the PivotTable is available on the view of Excel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableWizard(boolean value) {#setEnableWizard-boolean-}
```
public void setEnableWizard(boolean value)
```


Indicates whether the PivotTable Wizard is available.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setErrorString(String value) {#setErrorString-java.lang.String-}
```
public void setErrorString(String value)
```


Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setExcel2003Compatible(boolean value) {#setExcel2003Compatible-boolean-}
```
public void setExcel2003Compatible(boolean value)
```


Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFieldListSortAscending(boolean value) {#setFieldListSortAscending-boolean-}
```
public void setFieldListSortAscending(boolean value)
```


Indicates whether fields in the PivotTable are sorted in non-default order in the field list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setGrandTotalName(String value) {#setGrandTotalName-java.lang.String-}
```
public void setGrandTotalName(String value)
```


Returns the label that is displayed in the grand total column or row heading. The default value is the string "Grand Total".

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setGridDropZones(boolean value) {#setGridDropZones-boolean-}
```
public void setGridDropZones(boolean value)
```


Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasBlankRows(boolean value) {#setHasBlankRows-boolean-}
```
public void setHasBlankRows(boolean value)
```


Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIndent(int value) {#setIndent-int-}
```
public void setIndent(int value)
```


Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setItemPrintTitles(boolean value) {#setItemPrintTitles-boolean-}
```
public void setItemPrintTitles(boolean value)
```


Indicates whether PivotItem names should be repeated at the top of each printed page.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.RepeatItemsOnEachPrintedPage property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setManualGroupField(PivotField pivotField, DateTime startVal, DateTime endVal, ArrayList groupByList, int intervalNum) {#setManualGroupField-com.aspose.cells.PivotField-com.aspose.cells.DateTime-com.aspose.cells.DateTime-java.util.ArrayList-int-}
```
public void setManualGroupField(PivotField pivotField, DateTime startVal, DateTime endVal, ArrayList groupByList, int intervalNum)
```


Sets manual field group by the PivotTable.

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | The row or column field in the base fields |
| startVal | [DateTime](../../com.aspose.cells/datetime) | Specifies the starting value for date grouping. |
| endVal | [DateTime](../../com.aspose.cells/datetime) | Specifies the ending value for date grouping. |
| groupByList | java.util.ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | int | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |

### setManualGroupField(PivotField pivotField, double startVal, double endVal, ArrayList groupByList, double intervalNum) {#setManualGroupField-com.aspose.cells.PivotField-double-double-java.util.ArrayList-double-}
```
public void setManualGroupField(PivotField pivotField, double startVal, double endVal, ArrayList groupByList, double intervalNum)
```


Sets manual field group by the PivotTable.

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | The row or column field in the base fields |
| startVal | double | Specifies the starting value for numeric grouping. |
| endVal | double | Specifies the ending value for numeric grouping. |
| groupByList | java.util.ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | double | Specifies the interval number group by numeric grouping. |

### setManualGroupField(int baseFieldIndex, DateTime startVal, DateTime endVal, ArrayList groupByList, int intervalNum) {#setManualGroupField-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-java.util.ArrayList-int-}
```
public void setManualGroupField(int baseFieldIndex, DateTime startVal, DateTime endVal, ArrayList groupByList, int intervalNum)
```


Sets manual field group by the PivotTable.

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The row or column field index in the base fields |
| startVal | [DateTime](../../com.aspose.cells/datetime) | Specifies the starting value for date grouping. |
| endVal | [DateTime](../../com.aspose.cells/datetime) | Specifies the ending value for date grouping. |
| groupByList | java.util.ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | int | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |

### setManualGroupField(int baseFieldIndex, double startVal, double endVal, ArrayList groupByList, double intervalNum) {#setManualGroupField-int-double-double-java.util.ArrayList-double-}
```
public void setManualGroupField(int baseFieldIndex, double startVal, double endVal, ArrayList groupByList, double intervalNum)
```


Sets manual field group by the PivotTable.

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The row or column field index in the base fields |
| startVal | double | Specifies the starting value for numeric grouping. |
| endVal | double | Specifies the ending value for numeric grouping. |
| groupByList | java.util.ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | double | Specifies the interval number group by numeric grouping. |

### setManualUpdate(boolean value) {#setManualUpdate-boolean-}
```
public void setManualUpdate(boolean value)
```


Indicates whether the PivotTable report is recalculated only at the user's request.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMergeLabels(boolean value) {#setMergeLabels-boolean-}
```
public void setMergeLabels(boolean value)
```


True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

See [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMultipleFieldFilters(boolean value) {#setMultipleFieldFilters-boolean-}
```
public void setMultipleFieldFilters(boolean value)
```


Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.AllowMultipleFiltersPerField property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Gets the name of the PivotTable

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNullString(String value) {#setNullString-java.lang.String-}
```
public void setNullString(String value)
```


Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPageFieldOrder(int value) {#setPageFieldOrder-int-}
```
public void setPageFieldOrder(int value)
```


Sets the order in which page fields are added to the PivotTable report's layout.

See [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPageFieldWrapCount(int value) {#setPageFieldWrapCount-int-}
```
public void setPageFieldWrapCount(int value)
```


Gets the number of page fields in each column or row in the PivotTable report.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPivotTableStyle(TableStyle value) {#setPivotTableStyle-com.aspose.cells.TableStyle-}
```
public void setPivotTableStyle(TableStyle value)
```


Gets [TableStyle](../../com.aspose.cells/tablestyle) settings of this pivot table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TableStyle](../../com.aspose.cells/tablestyle) |  |

### setPivotTableStyleName(String value) {#setPivotTableStyleName-java.lang.String-}
```
public void setPivotTableStyleName(String value)
```


Sets the pivottable style name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPivotTableStyleType(int value) {#setPivotTableStyleType-int-}
```
public void setPivotTableStyleType(int value)
```


Sets the built-in pivot table style.

See [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPrintDrill(boolean value) {#setPrintDrill-boolean-}
```
public void setPrintDrill(boolean value)
```


Specifies a boolean value that indicates whether drill indicators should be printed. Print expand/collapse buttons when displayed on pivottable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPrintTitles(boolean value) {#setPrintTitles-boolean-}
```
public void setPrintTitles(boolean value)
```


Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRefreshDataFlag(boolean value) {#setRefreshDataFlag-boolean-}
```
public void setRefreshDataFlag(boolean value)
```


Indicates whether Refreshing Data or not.

**Remarks**

NOTE: This method is now obsolete. Instead, This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRefreshDataOnOpeningFile(boolean value) {#setRefreshDataOnOpeningFile-boolean-}
```
public void setRefreshDataOnOpeningFile(boolean value)
```


Indicates whether Refresh Data when Opening File.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRepeatItemsOnEachPrintedPage(boolean value) {#setRepeatItemsOnEachPrintedPage-boolean-}
```
public void setRepeatItemsOnEachPrintedPage(boolean value)
```


Indicates whether captions of pivot item on the row area are repeated on each printed page for pivot fields in tabular form.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRowGrand(boolean value) {#setRowGrand-boolean-}
```
public void setRowGrand(boolean value)
```


Indicates whether to show grand totals for rows of this pivot table.

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotTable.ShowRowGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRowHeaderCaption(String value) {#setRowHeaderCaption-java.lang.String-}
```
public void setRowHeaderCaption(String value)
```


Sets custom caption of the Row Header in this PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Indicates whether data for the PivotTable report is saved with the workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indicates whether this PivotTable is selected.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowColumnGrandTotals(boolean value) {#setShowColumnGrandTotals-boolean-}
```
public void setShowColumnGrandTotals(boolean value)
```


Indicates whether to show grand totals for columns of this pivot table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowDataTips(boolean value) {#setShowDataTips-boolean-}
```
public void setShowDataTips(boolean value)
```


Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowDrill(boolean value) {#setShowDrill-boolean-}
```
public void setShowDrill(boolean value)
```


Sets whether showing expand/collapse buttons.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowEmptyCol(boolean value) {#setShowEmptyCol-boolean-}
```
public void setShowEmptyCol(boolean value)
```


Indicates whether to include empty columns in the table

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowEmptyRow(boolean value) {#setShowEmptyRow-boolean-}
```
public void setShowEmptyRow(boolean value)
```


Indicates whether to include empty rows in the table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowMemberPropertyTips(boolean value) {#setShowMemberPropertyTips-boolean-}
```
public void setShowMemberPropertyTips(boolean value)
```


Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowPivotStyleColumnHeader(boolean value) {#setShowPivotStyleColumnHeader-boolean-}
```
public void setShowPivotStyleColumnHeader(boolean value)
```


Indicates whether the column header in the pivot table should have the style applied.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowPivotStyleColumnStripes(boolean value) {#setShowPivotStyleColumnStripes-boolean-}
```
public void setShowPivotStyleColumnStripes(boolean value)
```


Indicates whether stripe formatting is applied for column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowPivotStyleLastColumn(boolean value) {#setShowPivotStyleLastColumn-boolean-}
```
public void setShowPivotStyleLastColumn(boolean value)
```


Indicates whether the column formatting is applied.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowPivotStyleRowHeader(boolean value) {#setShowPivotStyleRowHeader-boolean-}
```
public void setShowPivotStyleRowHeader(boolean value)
```


Indicates whether the row header in the pivot table should have the style applied.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowPivotStyleRowStripes(boolean value) {#setShowPivotStyleRowStripes-boolean-}
```
public void setShowPivotStyleRowStripes(boolean value)
```


Indicates whether row stripe formatting is applied.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowRowGrandTotals(boolean value) {#setShowRowGrandTotals-boolean-}
```
public void setShowRowGrandTotals(boolean value)
```


Indicates whether to show grand totals for rows of the pivot table.

**Remarks**

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowRowHeaderCaption(boolean value) {#setShowRowHeaderCaption-boolean-}
```
public void setShowRowHeaderCaption(boolean value)
```


Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowValuesRow(boolean value) {#setShowValuesRow-boolean-}
```
public void setShowValuesRow(boolean value)
```


Indicates whether showing values row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSubtotalHiddenPageItems(boolean value) {#setSubtotalHiddenPageItems-boolean-}
```
public void setSubtotalHiddenPageItems(boolean value)
```


Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTag(String value) {#setTag-java.lang.String-}
```
public void setTag(String value)
```


Sets a user-defined string that is associated with this PivotTable view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setUngroup(PivotField pivotField) {#setUngroup-com.aspose.cells.PivotField-}
```
public void setUngroup(PivotField pivotField)
```


Sets ungroup by the PivotTable

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | The row or column field in the base fields |

### setUngroup(int baseFieldIndex) {#setUngroup-int-}
```
public void setUngroup(int baseFieldIndex)
```


Sets ungroup by the PivotTable

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The row or column field index in the base fields |

### showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn) {#showDetail-int-int-boolean-int-int-}
```
public void showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)
```


Show the detail of one item in the data region to a new Table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | Offset to the first data row in the data region. |
| columnOffset | int | Offset to the first data column in the data region. |
| newSheet | boolean | Show the detail to a new worksheet. |
| destRow | int | The target row. |
| destColumn | int | The target column. |

### showInCompactForm() {#showInCompactForm--}
```
public void showInCompactForm()
```


Layouts the PivotTable view in compact form.

### showInOutlineForm() {#showInOutlineForm--}
```
public void showInOutlineForm()
```


Layouts the PivotTable in outline form.

### showInTabularForm() {#showInTabularForm--}
```
public void showInTabularForm()
```


Layouts the PivotTable in tabular form.

### showReportFilterPage(PivotField pageField) {#showReportFilterPage-com.aspose.cells.PivotField-}
```
public void showReportFilterPage(PivotField pageField)
```


Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageField | [PivotField](../../com.aspose.cells/pivotfield) | The PivotField object |

### showReportFilterPageByIndex(int posIndex) {#showReportFilterPageByIndex-int-}
```
public void showReportFilterPageByIndex(int posIndex)
```


Show all the report filter pages according to the position index in the PageFields

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| posIndex | int | The position index in the PageFields |

### showReportFilterPageByName(String fieldName) {#showReportFilterPageByName-java.lang.String-}
```
public void showReportFilterPageByName(String fieldName)
```


Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | The name of PivotField |

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

