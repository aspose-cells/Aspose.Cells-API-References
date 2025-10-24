##PivotTable
Summary description for PivotTable.
## PivotTable class
Summary description for PivotTable.
```javascript
class PivotTable;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isExcel2003Compatible](#isExcel2003Compatible--)| boolean | Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true. |
| [refreshedByWho](#refreshedByWho--)| string | Readonly. Gets the name of the last user who refreshed this PivotTable |
| [refreshDate](#refreshDate--)| Date | Readonly. Gets the last date time when the PivotTable was refreshed. |
| [pivotTableStyleName](#pivotTableStyleName--)| string | Gets and sets the pivottable style name. |
| [pivotTableStyleType](#pivotTableStyleType--)| PivotTableStyleType | Gets and sets the built-in pivot table style. |
| [columnFields](#columnFields--)| PivotFieldCollection | Readonly. Returns a PivotFields object that are currently shown as column fields. |
| [rowFields](#rowFields--)| PivotFieldCollection | Readonly. Returns a PivotFields object that are currently shown as row fields. |
| [pageFields](#pageFields--)| PivotFieldCollection | Readonly. Returns a PivotFields object that are currently shown as page fields. |
| [dataFields](#dataFields--)| PivotFieldCollection | Readonly. Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area. |
| [dataField](#dataField--)| PivotField | Readonly. Gets a [PivotField](../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method . |
| [baseFields](#baseFields--)| PivotFieldCollection | Readonly. Returns all base pivot fields in the PivotTable. |
| [pivotFilters](#pivotFilters--)| PivotFilterCollection | Readonly. Returns all filters of pivot fields in the pivot table. |
| [columnRange](#columnRange--)| CellArea | Readonly. Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only. |
| [rowRange](#rowRange--)| CellArea | Readonly. Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only. |
| [dataBodyRange](#dataBodyRange--)| CellArea | Readonly. Returns a [CellArea](../cellarea/) object that represents the range that contains the data area in the list between the header row and the insert row. Read-only. |
| [tableRange1](#tableRange1--)| CellArea | Readonly. Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only. |
| [tableRange2](#tableRange2--)| CellArea | Readonly. Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only. |
| [isGridDropZones](#isGridDropZones--)| boolean | Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid) |
| [showColumnGrandTotals](#showColumnGrandTotals--)| boolean | Indicates whether to show grand totals for columns of this pivot table. |
| [showRowGrandTotals](#showRowGrandTotals--)| boolean | Indicates whether to show grand totals for rows of the pivot table. |
| [columnGrand](#columnGrand--)| boolean | Indicates whether the PivotTable report shows grand totals for columns. |
| [rowGrand](#rowGrand--)| boolean | Indicates whether to show grand totals for rows of this pivot table. |
| [displayNullString](#displayNullString--)| boolean | Indicates whether the PivotTable report displays a custom string if the value is null. |
| [nullString](#nullString--)| string | Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [displayErrorString](#displayErrorString--)| boolean | Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [dataFieldHeaderName](#dataFieldHeaderName--)| string | Gets and sets the name of the value area field header in the PivotTable. |
| [errorString](#errorString--)| string | Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [isAutoFormat](#isAutoFormat--)| boolean | Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003 |
| [autofitColumnWidthOnUpdate](#autofitColumnWidthOnUpdate--)| boolean | Indicates whether autofitting column width on update |
| [autoFormatType](#autoFormatType--)| PivotTableAutoFormatType | Gets and sets the auto format type of PivotTable. |
| [hasBlankRows](#hasBlankRows--)| boolean | Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows. |
| [mergeLabels](#mergeLabels--)| boolean | True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [preserveFormatting](#preserveFormatting--)| boolean | Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [showDrill](#showDrill--)| boolean | Gets and sets whether showing expand/collapse buttons. |
| [enableDrilldown](#enableDrilldown--)| boolean | Gets whether drilldown is enabled. |
| [enableFieldDialog](#enableFieldDialog--)| boolean | Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [enableFieldList](#enableFieldList--)| boolean | Indicates whether the field list for the PivotTable is available on the view of Excel. |
| [enableWizard](#enableWizard--)| boolean | Indicates whether the PivotTable Wizard is available. |
| [subtotalHiddenPageItems](#subtotalHiddenPageItems--)| boolean | Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False. |
| [grandTotalName](#grandTotalName--)| string | Returns the label that is displayed in the grand total column or row heading. The default value is the string "Grand Total". |
| [manualUpdate](#manualUpdate--)| boolean | Indicates whether the PivotTable report is recalculated only at the user's request. |
| [isMultipleFieldFilters](#isMultipleFieldFilters--)| boolean | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [allowMultipleFiltersPerField](#allowMultipleFiltersPerField--)| boolean | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [missingItemsLimit](#missingItemsLimit--)| PivotMissingItemLimitType | Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [enableDataValueEditing](#enableDataValueEditing--)| boolean | Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area |
| [showDataTips](#showDataTips--)| boolean | Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [showMemberPropertyTips](#showMemberPropertyTips--)| boolean | Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [showValuesRow](#showValuesRow--)| boolean | Indicates whether showing values row. |
| [showEmptyCol](#showEmptyCol--)| boolean | Indicates whether to include empty columns in the table |
| [showEmptyRow](#showEmptyRow--)| boolean | Indicates whether to include empty rows in the table. |
| [fieldListSortAscending](#fieldListSortAscending--)| boolean | Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [printDrill](#printDrill--)| boolean | Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable. |
| [altTextTitle](#altTextTitle--)| string | Gets and sets the title of the alter text. |
| [altTextDescription](#altTextDescription--)| string | Gets the description of the alt text. |
| [name](#name--)| string | Gets the name of the PivotTable |
| [columnHeaderCaption](#columnHeaderCaption--)| string | Gets the Column Header Caption of the PivotTable. |
| [indent](#indent--)| number | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [rowHeaderCaption](#rowHeaderCaption--)| string | Gets the Row Header Caption of the PivotTable. |
| [showRowHeaderCaption](#showRowHeaderCaption--)| boolean | Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs |
| [customListSort](#customListSort--)| boolean | Indicates whether consider built-in custom list when sort data |
| [pivotFormatConditions](#pivotFormatConditions--)| PivotFormatConditionCollection | Readonly. Gets the Format Conditions of the pivot table. |
| [conditionalFormats](#conditionalFormats--)| PivotConditionalFormatCollection | Readonly. Gets the conditional formats of the pivot table. |
| [pageFieldOrder](#pageFieldOrder--)| PrintOrderType | Gets and sets the order in which page fields are added to the PivotTable report's layout. |
| [pageFieldWrapCount](#pageFieldWrapCount--)| number | Gets the number of page fields in each column or row in the PivotTable report. |
| [tag](#tag--)| string | Gets a string saved with the PivotTable report. |
| [saveData](#saveData--)| boolean | Indicates whether data for the PivotTable report is saved with the workbook. |
| [refreshDataOnOpeningFile](#refreshDataOnOpeningFile--)| boolean | Indicates whether Refresh Data when Opening File. |
| [refreshDataFlag](#refreshDataFlag--)| boolean | Indicates whether Refreshing Data or not. |
| [sourceType](#sourceType--)| PivotTableSourceType | Readonly. Gets the data source type of the pivot table. |
| [externalConnectionDataSource](#externalConnectionDataSource--)| ExternalConnection | Readonly. Gets the external connection data source. |
| [dataSource](#dataSource--)| string[] | Gets and sets the data source of the pivot table. |
| [pivotFormats](#pivotFormats--)| PivotTableFormatCollection | Readonly. Gets the collection of formats applied to PivotTable. |
| [itemPrintTitles](#itemPrintTitles--)| boolean | Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [repeatItemsOnEachPrintedPage](#repeatItemsOnEachPrintedPage--)| boolean | Indicates whether pivot item captions on the row area are repeated on each printed page for pivot fields in tabular form. |
| [printTitles](#printTitles--)| boolean | Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false. |
| [displayImmediateItems](#displayImmediateItems--)| boolean | Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true. |
| [isSelected](#isSelected--)| boolean | Indicates whether this PivotTable is selected. |
| [showPivotStyleRowHeader](#showPivotStyleRowHeader--)| boolean | Indicates whether the row header in the pivot table should have the style applied. |
| [showPivotStyleColumnHeader](#showPivotStyleColumnHeader--)| boolean | Indicates whether the column header in the pivot table should have the style applied. |
| [showPivotStyleRowStripes](#showPivotStyleRowStripes--)| boolean | Indicates whether row stripe formatting is applied. |
| [showPivotStyleColumnStripes](#showPivotStyleColumnStripes--)| boolean | Indicates whether stripe formatting is applied for column. |
| [showPivotStyleLastColumn](#showPivotStyleLastColumn--)| boolean | Indicates whether the column formatting is applied. |
## Methods
| Method | Description |
| --- | --- |
| [isExcel2003Compatible()](#isExcel2003Compatible--)| <b>@deprecated.</b> Please use the 'isExcel2003Compatible' property instead. Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true. |
| [setIsExcel2003Compatible(boolean)](#setIsExcel2003Compatible-boolean-)| <b>@deprecated.</b> Please use the 'isExcel2003Compatible' property instead. Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true. |
| [getRefreshedByWho()](#getRefreshedByWho--)| <b>@deprecated.</b> Please use the 'refreshedByWho' property instead. Gets the name of the last user who refreshed this PivotTable |
| [getRefreshDate()](#getRefreshDate--)| <b>@deprecated.</b> Please use the 'refreshDate' property instead. Gets the last date time when the PivotTable was refreshed. |
| [getPivotTableStyleName()](#getPivotTableStyleName--)| <b>@deprecated.</b> Please use the 'pivotTableStyleName' property instead. Gets and sets the pivottable style name. |
| [setPivotTableStyleName(string)](#setPivotTableStyleName-string-)| <b>@deprecated.</b> Please use the 'pivotTableStyleName' property instead. Gets and sets the pivottable style name. |
| [getPivotTableStyleType()](#getPivotTableStyleType--)| <b>@deprecated.</b> Please use the 'pivotTableStyleType' property instead. Gets and sets the built-in pivot table style. |
| [setPivotTableStyleType(PivotTableStyleType)](#setPivotTableStyleType-pivottablestyletype-)| <b>@deprecated.</b> Please use the 'pivotTableStyleType' property instead. Gets and sets the built-in pivot table style. |
| [getColumnFields()](#getColumnFields--)| <b>@deprecated.</b> Please use the 'columnFields' property instead. Returns a PivotFields object that are currently shown as column fields. |
| [getRowFields()](#getRowFields--)| <b>@deprecated.</b> Please use the 'rowFields' property instead. Returns a PivotFields object that are currently shown as row fields. |
| [getPageFields()](#getPageFields--)| <b>@deprecated.</b> Please use the 'pageFields' property instead. Returns a PivotFields object that are currently shown as page fields. |
| [getDataFields()](#getDataFields--)| <b>@deprecated.</b> Please use the 'dataFields' property instead. Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area. |
| [getDataField()](#getDataField--)| <b>@deprecated.</b> Please use the 'dataField' property instead. Gets a [PivotField](../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method . |
| [getBaseFields()](#getBaseFields--)| <b>@deprecated.</b> Please use the 'baseFields' property instead. Returns all base pivot fields in the PivotTable. |
| [getPivotFilters()](#getPivotFilters--)| <b>@deprecated.</b> Please use the 'pivotFilters' property instead. Returns all filters of pivot fields in the pivot table. |
| [getColumnRange()](#getColumnRange--)| <b>@deprecated.</b> Please use the 'columnRange' property instead. Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only. |
| [getRowRange()](#getRowRange--)| <b>@deprecated.</b> Please use the 'rowRange' property instead. Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only. |
| [getDataBodyRange()](#getDataBodyRange--)| <b>@deprecated.</b> Please use the 'dataBodyRange' property instead. Returns a [CellArea](../cellarea/) object that represents the range that contains the data area in the list between the header row and the insert row. Read-only. |
| [getTableRange1()](#getTableRange1--)| <b>@deprecated.</b> Please use the 'tableRange1' property instead. Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only. |
| [getTableRange2()](#getTableRange2--)| <b>@deprecated.</b> Please use the 'tableRange2' property instead. Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only. |
| [isGridDropZones()](#isGridDropZones--)| <b>@deprecated.</b> Please use the 'isGridDropZones' property instead. Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid) |
| [setIsGridDropZones(boolean)](#setIsGridDropZones-boolean-)| <b>@deprecated.</b> Please use the 'isGridDropZones' property instead. Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid) |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--)| <b>@deprecated.</b> Please use the 'showColumnGrandTotals' property instead. Indicates whether to show grand totals for columns of this pivot table. |
| [setShowColumnGrandTotals(boolean)](#setShowColumnGrandTotals-boolean-)| <b>@deprecated.</b> Please use the 'showColumnGrandTotals' property instead. Indicates whether to show grand totals for columns of this pivot table. |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--)| <b>@deprecated.</b> Please use the 'showRowGrandTotals' property instead. Indicates whether to show grand totals for rows of the pivot table. |
| [setShowRowGrandTotals(boolean)](#setShowRowGrandTotals-boolean-)| <b>@deprecated.</b> Please use the 'showRowGrandTotals' property instead. Indicates whether to show grand totals for rows of the pivot table. |
| [getColumnGrand()](#getColumnGrand--)| <b>@deprecated.</b> Please use the 'columnGrand' property instead. Indicates whether the PivotTable report shows grand totals for columns. |
| [setColumnGrand(boolean)](#setColumnGrand-boolean-)| <b>@deprecated.</b> Please use the 'columnGrand' property instead. Indicates whether the PivotTable report shows grand totals for columns. |
| [getRowGrand()](#getRowGrand--)| <b>@deprecated.</b> Please use the 'rowGrand' property instead. Indicates whether to show grand totals for rows of this pivot table. |
| [setRowGrand(boolean)](#setRowGrand-boolean-)| <b>@deprecated.</b> Please use the 'rowGrand' property instead. Indicates whether to show grand totals for rows of this pivot table. |
| [getDisplayNullString()](#getDisplayNullString--)| <b>@deprecated.</b> Please use the 'displayNullString' property instead. Indicates whether the PivotTable report displays a custom string if the value is null. |
| [setDisplayNullString(boolean)](#setDisplayNullString-boolean-)| <b>@deprecated.</b> Please use the 'displayNullString' property instead. Indicates whether the PivotTable report displays a custom string if the value is null. |
| [getNullString()](#getNullString--)| <b>@deprecated.</b> Please use the 'nullString' property instead. Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [setNullString(string)](#setNullString-string-)| <b>@deprecated.</b> Please use the 'nullString' property instead. Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [getDisplayErrorString()](#getDisplayErrorString--)| <b>@deprecated.</b> Please use the 'displayErrorString' property instead. Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [setDisplayErrorString(boolean)](#setDisplayErrorString-boolean-)| <b>@deprecated.</b> Please use the 'displayErrorString' property instead. Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--)| <b>@deprecated.</b> Please use the 'dataFieldHeaderName' property instead. Gets and sets the name of the value area field header in the PivotTable. |
| [setDataFieldHeaderName(string)](#setDataFieldHeaderName-string-)| <b>@deprecated.</b> Please use the 'dataFieldHeaderName' property instead. Gets and sets the name of the value area field header in the PivotTable. |
| [getErrorString()](#getErrorString--)| <b>@deprecated.</b> Please use the 'errorString' property instead. Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [setErrorString(string)](#setErrorString-string-)| <b>@deprecated.</b> Please use the 'errorString' property instead. Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [isAutoFormat()](#isAutoFormat--)| <b>@deprecated.</b> Please use the 'isAutoFormat' property instead. Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003 |
| [setIsAutoFormat(boolean)](#setIsAutoFormat-boolean-)| <b>@deprecated.</b> Please use the 'isAutoFormat' property instead. Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003 |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--)| <b>@deprecated.</b> Please use the 'autofitColumnWidthOnUpdate' property instead. Indicates whether autofitting column width on update |
| [setAutofitColumnWidthOnUpdate(boolean)](#setAutofitColumnWidthOnUpdate-boolean-)| <b>@deprecated.</b> Please use the 'autofitColumnWidthOnUpdate' property instead. Indicates whether autofitting column width on update |
| [getAutoFormatType()](#getAutoFormatType--)| <b>@deprecated.</b> Please use the 'autoFormatType' property instead. Gets and sets the auto format type of PivotTable. |
| [setAutoFormatType(PivotTableAutoFormatType)](#setAutoFormatType-pivottableautoformattype-)| <b>@deprecated.</b> Please use the 'autoFormatType' property instead. Gets and sets the auto format type of PivotTable. |
| [getHasBlankRows()](#getHasBlankRows--)| <b>@deprecated.</b> Please use the 'hasBlankRows' property instead. Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows. |
| [setHasBlankRows(boolean)](#setHasBlankRows-boolean-)| <b>@deprecated.</b> Please use the 'hasBlankRows' property instead. Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows. |
| [getMergeLabels()](#getMergeLabels--)| <b>@deprecated.</b> Please use the 'mergeLabels' property instead. True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [setMergeLabels(boolean)](#setMergeLabels-boolean-)| <b>@deprecated.</b> Please use the 'mergeLabels' property instead. True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [getPreserveFormatting()](#getPreserveFormatting--)| <b>@deprecated.</b> Please use the 'preserveFormatting' property instead. Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [setPreserveFormatting(boolean)](#setPreserveFormatting-boolean-)| <b>@deprecated.</b> Please use the 'preserveFormatting' property instead. Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [getShowDrill()](#getShowDrill--)| <b>@deprecated.</b> Please use the 'showDrill' property instead. Gets and sets whether showing expand/collapse buttons. |
| [setShowDrill(boolean)](#setShowDrill-boolean-)| <b>@deprecated.</b> Please use the 'showDrill' property instead. Gets and sets whether showing expand/collapse buttons. |
| [getEnableDrilldown()](#getEnableDrilldown--)| <b>@deprecated.</b> Please use the 'enableDrilldown' property instead. Gets whether drilldown is enabled. |
| [setEnableDrilldown(boolean)](#setEnableDrilldown-boolean-)| <b>@deprecated.</b> Please use the 'enableDrilldown' property instead. Gets whether drilldown is enabled. |
| [getEnableFieldDialog()](#getEnableFieldDialog--)| <b>@deprecated.</b> Please use the 'enableFieldDialog' property instead. Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [setEnableFieldDialog(boolean)](#setEnableFieldDialog-boolean-)| <b>@deprecated.</b> Please use the 'enableFieldDialog' property instead. Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [getEnableFieldList()](#getEnableFieldList--)| <b>@deprecated.</b> Please use the 'enableFieldList' property instead. Indicates whether the field list for the PivotTable is available on the view of Excel. |
| [setEnableFieldList(boolean)](#setEnableFieldList-boolean-)| <b>@deprecated.</b> Please use the 'enableFieldList' property instead. Indicates whether the field list for the PivotTable is available on the view of Excel. |
| [getEnableWizard()](#getEnableWizard--)| <b>@deprecated.</b> Please use the 'enableWizard' property instead. Indicates whether the PivotTable Wizard is available. |
| [setEnableWizard(boolean)](#setEnableWizard-boolean-)| <b>@deprecated.</b> Please use the 'enableWizard' property instead. Indicates whether the PivotTable Wizard is available. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--)| <b>@deprecated.</b> Please use the 'subtotalHiddenPageItems' property instead. Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False. |
| [setSubtotalHiddenPageItems(boolean)](#setSubtotalHiddenPageItems-boolean-)| <b>@deprecated.</b> Please use the 'subtotalHiddenPageItems' property instead. Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False. |
| [getGrandTotalName()](#getGrandTotalName--)| <b>@deprecated.</b> Please use the 'grandTotalName' property instead. Returns the label that is displayed in the grand total column or row heading. The default value is the string "Grand Total". |
| [setGrandTotalName(string)](#setGrandTotalName-string-)| <b>@deprecated.</b> Please use the 'grandTotalName' property instead. Returns the label that is displayed in the grand total column or row heading. The default value is the string "Grand Total". |
| [getManualUpdate()](#getManualUpdate--)| <b>@deprecated.</b> Please use the 'manualUpdate' property instead. Indicates whether the PivotTable report is recalculated only at the user's request. |
| [setManualUpdate(boolean)](#setManualUpdate-boolean-)| <b>@deprecated.</b> Please use the 'manualUpdate' property instead. Indicates whether the PivotTable report is recalculated only at the user's request. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--)| <b>@deprecated.</b> Please use the 'isMultipleFieldFilters' property instead. Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [setIsMultipleFieldFilters(boolean)](#setIsMultipleFieldFilters-boolean-)| <b>@deprecated.</b> Please use the 'isMultipleFieldFilters' property instead. Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--)| <b>@deprecated.</b> Please use the 'allowMultipleFiltersPerField' property instead. Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [setAllowMultipleFiltersPerField(boolean)](#setAllowMultipleFiltersPerField-boolean-)| <b>@deprecated.</b> Please use the 'allowMultipleFiltersPerField' property instead. Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [getMissingItemsLimit()](#getMissingItemsLimit--)| <b>@deprecated.</b> Please use the 'missingItemsLimit' property instead. Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [setMissingItemsLimit(PivotMissingItemLimitType)](#setMissingItemsLimit-pivotmissingitemlimittype-)| <b>@deprecated.</b> Please use the 'missingItemsLimit' property instead. Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--)| <b>@deprecated.</b> Please use the 'enableDataValueEditing' property instead. Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area |
| [setEnableDataValueEditing(boolean)](#setEnableDataValueEditing-boolean-)| <b>@deprecated.</b> Please use the 'enableDataValueEditing' property instead. Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area |
| [getShowDataTips()](#getShowDataTips--)| <b>@deprecated.</b> Please use the 'showDataTips' property instead. Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [setShowDataTips(boolean)](#setShowDataTips-boolean-)| <b>@deprecated.</b> Please use the 'showDataTips' property instead. Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--)| <b>@deprecated.</b> Please use the 'showMemberPropertyTips' property instead. Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [setShowMemberPropertyTips(boolean)](#setShowMemberPropertyTips-boolean-)| <b>@deprecated.</b> Please use the 'showMemberPropertyTips' property instead. Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [getShowValuesRow()](#getShowValuesRow--)| <b>@deprecated.</b> Please use the 'showValuesRow' property instead. Indicates whether showing values row. |
| [setShowValuesRow(boolean)](#setShowValuesRow-boolean-)| <b>@deprecated.</b> Please use the 'showValuesRow' property instead. Indicates whether showing values row. |
| [getShowEmptyCol()](#getShowEmptyCol--)| <b>@deprecated.</b> Please use the 'showEmptyCol' property instead. Indicates whether to include empty columns in the table |
| [setShowEmptyCol(boolean)](#setShowEmptyCol-boolean-)| <b>@deprecated.</b> Please use the 'showEmptyCol' property instead. Indicates whether to include empty columns in the table |
| [getShowEmptyRow()](#getShowEmptyRow--)| <b>@deprecated.</b> Please use the 'showEmptyRow' property instead. Indicates whether to include empty rows in the table. |
| [setShowEmptyRow(boolean)](#setShowEmptyRow-boolean-)| <b>@deprecated.</b> Please use the 'showEmptyRow' property instead. Indicates whether to include empty rows in the table. |
| [getFieldListSortAscending()](#getFieldListSortAscending--)| <b>@deprecated.</b> Please use the 'fieldListSortAscending' property instead. Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [setFieldListSortAscending(boolean)](#setFieldListSortAscending-boolean-)| <b>@deprecated.</b> Please use the 'fieldListSortAscending' property instead. Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [getPrintDrill()](#getPrintDrill--)| <b>@deprecated.</b> Please use the 'printDrill' property instead. Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable. |
| [setPrintDrill(boolean)](#setPrintDrill-boolean-)| <b>@deprecated.</b> Please use the 'printDrill' property instead. Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable. |
| [getAltTextTitle()](#getAltTextTitle--)| <b>@deprecated.</b> Please use the 'altTextTitle' property instead. Gets and sets the title of the alter text. |
| [setAltTextTitle(string)](#setAltTextTitle-string-)| <b>@deprecated.</b> Please use the 'altTextTitle' property instead. Gets and sets the title of the alter text. |
| [getAltTextDescription()](#getAltTextDescription--)| <b>@deprecated.</b> Please use the 'altTextDescription' property instead. Gets the description of the alt text. |
| [setAltTextDescription(string)](#setAltTextDescription-string-)| <b>@deprecated.</b> Please use the 'altTextDescription' property instead. Gets the description of the alt text. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the PivotTable |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the PivotTable |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--)| <b>@deprecated.</b> Please use the 'columnHeaderCaption' property instead. Gets the Column Header Caption of the PivotTable. |
| [setColumnHeaderCaption(string)](#setColumnHeaderCaption-string-)| <b>@deprecated.</b> Please use the 'columnHeaderCaption' property instead. Gets the Column Header Caption of the PivotTable. |
| [getIndent()](#getIndent--)| <b>@deprecated.</b> Please use the 'indent' property instead. Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [setIndent(number)](#setIndent-number-)| <b>@deprecated.</b> Please use the 'indent' property instead. Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [getRowHeaderCaption()](#getRowHeaderCaption--)| <b>@deprecated.</b> Please use the 'rowHeaderCaption' property instead. Gets the Row Header Caption of the PivotTable. |
| [setRowHeaderCaption(string)](#setRowHeaderCaption-string-)| <b>@deprecated.</b> Please use the 'rowHeaderCaption' property instead. Gets the Row Header Caption of the PivotTable. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--)| <b>@deprecated.</b> Please use the 'showRowHeaderCaption' property instead. Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs |
| [setShowRowHeaderCaption(boolean)](#setShowRowHeaderCaption-boolean-)| <b>@deprecated.</b> Please use the 'showRowHeaderCaption' property instead. Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs |
| [getCustomListSort()](#getCustomListSort--)| <b>@deprecated.</b> Please use the 'customListSort' property instead. Indicates whether consider built-in custom list when sort data |
| [setCustomListSort(boolean)](#setCustomListSort-boolean-)| <b>@deprecated.</b> Please use the 'customListSort' property instead. Indicates whether consider built-in custom list when sort data |
| [getPivotFormatConditions()](#getPivotFormatConditions--)| <b>@deprecated.</b> Please use the 'pivotFormatConditions' property instead. Gets the Format Conditions of the pivot table. |
| [getConditionalFormats()](#getConditionalFormats--)| <b>@deprecated.</b> Please use the 'conditionalFormats' property instead. Gets the conditional formats of the pivot table. |
| [getPageFieldOrder()](#getPageFieldOrder--)| <b>@deprecated.</b> Please use the 'pageFieldOrder' property instead. Gets and sets the order in which page fields are added to the PivotTable report's layout. |
| [setPageFieldOrder(PrintOrderType)](#setPageFieldOrder-printordertype-)| <b>@deprecated.</b> Please use the 'pageFieldOrder' property instead. Gets and sets the order in which page fields are added to the PivotTable report's layout. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--)| <b>@deprecated.</b> Please use the 'pageFieldWrapCount' property instead. Gets the number of page fields in each column or row in the PivotTable report. |
| [setPageFieldWrapCount(number)](#setPageFieldWrapCount-number-)| <b>@deprecated.</b> Please use the 'pageFieldWrapCount' property instead. Gets the number of page fields in each column or row in the PivotTable report. |
| [getTag()](#getTag--)| <b>@deprecated.</b> Please use the 'tag' property instead. Gets a string saved with the PivotTable report. |
| [setTag(string)](#setTag-string-)| <b>@deprecated.</b> Please use the 'tag' property instead. Gets a string saved with the PivotTable report. |
| [getSaveData()](#getSaveData--)| <b>@deprecated.</b> Please use the 'saveData' property instead. Indicates whether data for the PivotTable report is saved with the workbook. |
| [setSaveData(boolean)](#setSaveData-boolean-)| <b>@deprecated.</b> Please use the 'saveData' property instead. Indicates whether data for the PivotTable report is saved with the workbook. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--)| <b>@deprecated.</b> Please use the 'refreshDataOnOpeningFile' property instead. Indicates whether Refresh Data when Opening File. |
| [setRefreshDataOnOpeningFile(boolean)](#setRefreshDataOnOpeningFile-boolean-)| <b>@deprecated.</b> Please use the 'refreshDataOnOpeningFile' property instead. Indicates whether Refresh Data when Opening File. |
| [getRefreshDataFlag()](#getRefreshDataFlag--)| <b>@deprecated.</b> Please use the 'refreshDataFlag' property instead. Indicates whether Refreshing Data or not. |
| [setRefreshDataFlag(boolean)](#setRefreshDataFlag-boolean-)| <b>@deprecated.</b> Please use the 'refreshDataFlag' property instead. Indicates whether Refreshing Data or not. |
| [getSourceType()](#getSourceType--)| <b>@deprecated.</b> Please use the 'sourceType' property instead. Gets the data source type of the pivot table. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--)| <b>@deprecated.</b> Please use the 'externalConnectionDataSource' property instead. Gets the external connection data source. |
| [getDataSource()](#getDataSource--)| <b>@deprecated.</b> Please use the 'dataSource' property instead. Gets and sets the data source of the pivot table. |
| [setDataSource(string[])](#setDataSource-stringarray-)| <b>@deprecated.</b> Please use the 'dataSource' property instead. Gets and sets the data source of the pivot table. |
| [getPivotFormats()](#getPivotFormats--)| <b>@deprecated.</b> Please use the 'pivotFormats' property instead. Gets the collection of formats applied to PivotTable. |
| [getItemPrintTitles()](#getItemPrintTitles--)| <b>@deprecated.</b> Please use the 'itemPrintTitles' property instead. Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [setItemPrintTitles(boolean)](#setItemPrintTitles-boolean-)| <b>@deprecated.</b> Please use the 'itemPrintTitles' property instead. Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--)| <b>@deprecated.</b> Please use the 'repeatItemsOnEachPrintedPage' property instead. Indicates whether pivot item captions on the row area are repeated on each printed page for pivot fields in tabular form. |
| [setRepeatItemsOnEachPrintedPage(boolean)](#setRepeatItemsOnEachPrintedPage-boolean-)| <b>@deprecated.</b> Please use the 'repeatItemsOnEachPrintedPage' property instead. Indicates whether pivot item captions on the row area are repeated on each printed page for pivot fields in tabular form. |
| [getPrintTitles()](#getPrintTitles--)| <b>@deprecated.</b> Please use the 'printTitles' property instead. Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false. |
| [setPrintTitles(boolean)](#setPrintTitles-boolean-)| <b>@deprecated.</b> Please use the 'printTitles' property instead. Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--)| <b>@deprecated.</b> Please use the 'displayImmediateItems' property instead. Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true. |
| [setDisplayImmediateItems(boolean)](#setDisplayImmediateItems-boolean-)| <b>@deprecated.</b> Please use the 'displayImmediateItems' property instead. Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true. |
| [isSelected()](#isSelected--)| <b>@deprecated.</b> Please use the 'isSelected' property instead. Indicates whether this PivotTable is selected. |
| [setIsSelected(boolean)](#setIsSelected-boolean-)| <b>@deprecated.</b> Please use the 'isSelected' property instead. Indicates whether this PivotTable is selected. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--)| <b>@deprecated.</b> Please use the 'showPivotStyleRowHeader' property instead. Indicates whether the row header in the pivot table should have the style applied. |
| [setShowPivotStyleRowHeader(boolean)](#setShowPivotStyleRowHeader-boolean-)| <b>@deprecated.</b> Please use the 'showPivotStyleRowHeader' property instead. Indicates whether the row header in the pivot table should have the style applied. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--)| <b>@deprecated.</b> Please use the 'showPivotStyleColumnHeader' property instead. Indicates whether the column header in the pivot table should have the style applied. |
| [setShowPivotStyleColumnHeader(boolean)](#setShowPivotStyleColumnHeader-boolean-)| <b>@deprecated.</b> Please use the 'showPivotStyleColumnHeader' property instead. Indicates whether the column header in the pivot table should have the style applied. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--)| <b>@deprecated.</b> Please use the 'showPivotStyleRowStripes' property instead. Indicates whether row stripe formatting is applied. |
| [setShowPivotStyleRowStripes(boolean)](#setShowPivotStyleRowStripes-boolean-)| <b>@deprecated.</b> Please use the 'showPivotStyleRowStripes' property instead. Indicates whether row stripe formatting is applied. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--)| <b>@deprecated.</b> Please use the 'showPivotStyleColumnStripes' property instead. Indicates whether stripe formatting is applied for column. |
| [setShowPivotStyleColumnStripes(boolean)](#setShowPivotStyleColumnStripes-boolean-)| <b>@deprecated.</b> Please use the 'showPivotStyleColumnStripes' property instead. Indicates whether stripe formatting is applied for column. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--)| <b>@deprecated.</b> Please use the 'showPivotStyleLastColumn' property instead. Indicates whether the column formatting is applied. |
| [setShowPivotStyleLastColumn(boolean)](#setShowPivotStyleLastColumn-boolean-)| <b>@deprecated.</b> Please use the 'showPivotStyleLastColumn' property instead. Indicates whether the column formatting is applied. |
| [dispose()](#dispose--)| Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [copyStyle(PivotTable)](#copyStyle-pivottable-)| Copies named style from another pivot table. |
| [showReportFilterPage(PivotField)](#showReportFilterPage-pivotfield-)| Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields. |
| [showReportFilterPageByName(string)](#showReportFilterPageByName-string-)| Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields. |
| [showReportFilterPageByIndex(number)](#showReportFilterPageByIndex-number-)| Show all the report filter pages according to the position index in the PageFields |
| [removeField(PivotFieldType, string)](#removeField-pivotfieldtype-string-)| Removes a field from specific field area |
| [removeField(PivotFieldType, number)](#removeField-pivotfieldtype-number-)| Removes a field from specific field area |
| [removeField(PivotFieldType, PivotField)](#removeField-pivotfieldtype-pivotfield-)| Remove field from specific field area |
| [addFieldToArea(PivotFieldType, string)](#addFieldToArea-pivotfieldtype-string-)| Adds the field to the specific area. |
| [addFieldToArea(PivotFieldType, number)](#addFieldToArea-pivotfieldtype-number-)| Adds the field to the specific area. |
| [addFieldToArea(PivotFieldType, PivotField)](#addFieldToArea-pivotfieldtype-pivotfield-)| Adds the field to the specific area. |
| [addCalculatedField(string, string, boolean)](#addCalculatedField-string-string-boolean-)| Adds a calculated field to pivot field. |
| [addCalculatedField(string, string)](#addCalculatedField-string-string-)| Adds a calculated field to pivot field and drag it to data area. |
| [getFields(PivotFieldType)](#getFields-pivotfieldtype-)| Gets the specific pivot field list by the region. |
| [move(number, number)](#move-number-number-)| Moves the PivotTable to a different location in the worksheet. |
| [move(string)](#move-string-)| Moves the PivotTable to a different location in the worksheet. |
| [moveTo(number, number)](#moveTo-number-number-)| Moves the PivotTable to a different location in the worksheet. |
| [moveTo(string)](#moveTo-string-)| Moves the PivotTable to a different location in the worksheet. |
| [getSourceDataConnections()](#getSourceDataConnections--)| Gets the external connection data sources. |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--)| Gets the name of external source data connections. |
| [changeDataSource(string[])](#changeDataSource-stringarray-)| Set pivottable's source data. |
| [getSource()](#getSource--)| Get pivottable's source data. |
| [getSource(boolean)](#getSource-boolean-)| Get pivottable's source data. |
| [refreshData()](#refreshData--)| Refreshes pivottable's data and setting from it's data source. |
| [refreshData(PivotTableRefreshOption)](#refreshData-pivottablerefreshoption-)| Refreshes pivottable's data and setting from it's data source with options. |
| [calculateData()](#calculateData--)| Calculates pivottable's data to cells. |
| [calculateData(PivotTableCalculateOption)](#calculateData-pivottablecalculateoption-)| Calculating pivot tables with options |
| [clearData()](#clearData--)| Clear PivotTable's data and formatting |
| [calculateRange()](#calculateRange--)| Calculates pivottable's range. |
| [formatAll(Style)](#formatAll-style-)| Format all the cell in the pivottable area |
| [formatRow(number, Style)](#formatRow-number-style-)| Format the row data in the pivottable area |
| [format(PivotArea, Style)](#format-pivotarea-style-)| Formats selected area of the PivotTable. |
| [format(CellArea, Style)](#format-cellarea-style-)| Formats selected area of the PivotTable. |
| [format(number, number, Style)](#format-number-number-style-)| Format the cell in the pivottable area |
| [selectArea(CellArea)](#selectArea-cellarea-)| Select an area of pivot table view. |
| [showDetail(number, number, boolean, number, number)](#showDetail-number-number-boolean-number-number-)| Show the detail of one item in the data region to a new Table. |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--)| Gets horizontal page breaks of this pivot table. |
| [showInCompactForm()](#showInCompactForm--)| Layouts the PivotTable in compact form. |
| [showInOutlineForm()](#showInOutlineForm--)| Layouts the PivotTable in outline form. |
| [showInTabularForm()](#showInTabularForm--)| Layouts the PivotTable in tabular form. |
| [getCellByDisplayName(string)](#getCellByDisplayName-string-)| Gets the [Cell](../cell/) object by the display name of PivotField. |
| [getChildren()](#getChildren--)| Gets the Children Pivot Tables which use this PivotTable data as data source. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### isExcel2003Compatible {#isExcel2003Compatible--}
Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true.
```javascript
isExcel2003Compatible : boolean;
```
### refreshedByWho {#refreshedByWho--}
Readonly. Gets the name of the last user who refreshed this PivotTable
```javascript
refreshedByWho : string;
```
### refreshDate {#refreshDate--}
Readonly. Gets the last date time when the PivotTable was refreshed.
```javascript
refreshDate : Date;
```
### pivotTableStyleName {#pivotTableStyleName--}
Gets and sets the pivottable style name.
```javascript
pivotTableStyleName : string;
```
### pivotTableStyleType {#pivotTableStyleType--}
Gets and sets the built-in pivot table style.
```javascript
pivotTableStyleType : PivotTableStyleType;
```
### columnFields {#columnFields--}
Readonly. Returns a PivotFields object that are currently shown as column fields.
```javascript
columnFields : PivotFieldCollection;
```
### rowFields {#rowFields--}
Readonly. Returns a PivotFields object that are currently shown as row fields.
```javascript
rowFields : PivotFieldCollection;
```
### pageFields {#pageFields--}
Readonly. Returns a PivotFields object that are currently shown as page fields.
```javascript
pageFields : PivotFieldCollection;
```
### dataFields {#dataFields--}
Readonly. Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.
```javascript
dataFields : PivotFieldCollection;
```
### dataField {#dataField--}
Readonly. Gets a [PivotField](../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .
```javascript
dataField : PivotField;
```
### baseFields {#baseFields--}
Readonly. Returns all base pivot fields in the PivotTable.
```javascript
baseFields : PivotFieldCollection;
```
### pivotFilters {#pivotFilters--}
Readonly. Returns all filters of pivot fields in the pivot table.
```javascript
pivotFilters : PivotFilterCollection;
```
### columnRange {#columnRange--}
Readonly. Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only.
```javascript
columnRange : CellArea;
```
### rowRange {#rowRange--}
Readonly. Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only.
```javascript
rowRange : CellArea;
```
### dataBodyRange {#dataBodyRange--}
Readonly. Returns a [CellArea](../cellarea/) object that represents the range that contains the data area in the list between the header row and the insert row. Read-only.
```javascript
dataBodyRange : CellArea;
```
### tableRange1 {#tableRange1--}
Readonly. Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only.
```javascript
tableRange1 : CellArea;
```
### tableRange2 {#tableRange2--}
Readonly. Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only.
```javascript
tableRange2 : CellArea;
```
### isGridDropZones {#isGridDropZones--}
Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)
```javascript
isGridDropZones : boolean;
```
### showColumnGrandTotals {#showColumnGrandTotals--}
Indicates whether to show grand totals for columns of this pivot table.
```javascript
showColumnGrandTotals : boolean;
```
### showRowGrandTotals {#showRowGrandTotals--}
Indicates whether to show grand totals for rows of the pivot table.
```javascript
showRowGrandTotals : boolean;
```
### columnGrand {#columnGrand--}
Indicates whether the PivotTable report shows grand totals for columns.
```javascript
columnGrand : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.ShowColumnGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### rowGrand {#rowGrand--}
Indicates whether to show grand totals for rows of this pivot table.
```javascript
rowGrand : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.ShowRowGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### displayNullString {#displayNullString--}
Indicates whether the PivotTable report displays a custom string if the value is null.
```javascript
displayNullString : boolean;
```
### nullString {#nullString--}
Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string.
```javascript
nullString : string;
```
### displayErrorString {#displayErrorString--}
Indicates whether the PivotTable report displays a custom string in cells that contain errors.
```javascript
displayErrorString : boolean;
```
### dataFieldHeaderName {#dataFieldHeaderName--}
Gets and sets the name of the value area field header in the PivotTable.
```javascript
dataFieldHeaderName : string;
```
### errorString {#errorString--}
Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string.
```javascript
errorString : string;
```
### isAutoFormat {#isAutoFormat--}
Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003
```javascript
isAutoFormat : boolean;
```
### autofitColumnWidthOnUpdate {#autofitColumnWidthOnUpdate--}
Indicates whether autofitting column width on update
```javascript
autofitColumnWidthOnUpdate : boolean;
```
### autoFormatType {#autoFormatType--}
Gets and sets the auto format type of PivotTable.
```javascript
autoFormatType : PivotTableAutoFormatType;
```
### hasBlankRows {#hasBlankRows--}
Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.
```javascript
hasBlankRows : boolean;
```
### mergeLabels {#mergeLabels--}
True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells.
```javascript
mergeLabels : boolean;
```
### preserveFormatting {#preserveFormatting--}
Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated.
```javascript
preserveFormatting : boolean;
```
### showDrill {#showDrill--}
Gets and sets whether showing expand/collapse buttons.
```javascript
showDrill : boolean;
```
### enableDrilldown {#enableDrilldown--}
Gets whether drilldown is enabled.
```javascript
enableDrilldown : boolean;
```
### enableFieldDialog {#enableFieldDialog--}
Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field.
```javascript
enableFieldDialog : boolean;
```
### enableFieldList {#enableFieldList--}
Indicates whether the field list for the PivotTable is available on the view of Excel.
```javascript
enableFieldList : boolean;
```
### enableWizard {#enableWizard--}
Indicates whether the PivotTable Wizard is available.
```javascript
enableWizard : boolean;
```
### subtotalHiddenPageItems {#subtotalHiddenPageItems--}
Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False.
```javascript
subtotalHiddenPageItems : boolean;
```
### grandTotalName {#grandTotalName--}
Returns the label that is displayed in the grand total column or row heading. The default value is the string "Grand Total".
```javascript
grandTotalName : string;
```
### manualUpdate {#manualUpdate--}
Indicates whether the PivotTable report is recalculated only at the user's request.
```javascript
manualUpdate : boolean;
```
### isMultipleFieldFilters {#isMultipleFieldFilters--}
Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.
```javascript
isMultipleFieldFilters : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.AllowMultipleFiltersPerField property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### allowMultipleFiltersPerField {#allowMultipleFiltersPerField--}
Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.
```javascript
allowMultipleFiltersPerField : boolean;
```
### missingItemsLimit {#missingItemsLimit--}
Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.
```javascript
missingItemsLimit : PivotMissingItemLimitType;
```
### enableDataValueEditing {#enableDataValueEditing--}
Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area
```javascript
enableDataValueEditing : boolean;
```
### showDataTips {#showDataTips--}
Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells.
```javascript
showDataTips : boolean;
```
### showMemberPropertyTips {#showMemberPropertyTips--}
Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips.
```javascript
showMemberPropertyTips : boolean;
```
### showValuesRow {#showValuesRow--}
Indicates whether showing values row.
```javascript
showValuesRow : boolean;
```
### showEmptyCol {#showEmptyCol--}
Indicates whether to include empty columns in the table
```javascript
showEmptyCol : boolean;
```
### showEmptyRow {#showEmptyRow--}
Indicates whether to include empty rows in the table.
```javascript
showEmptyRow : boolean;
```
### fieldListSortAscending {#fieldListSortAscending--}
Indicates whether fields in the PivotTable are sorted in non-default order in the field list.
```javascript
fieldListSortAscending : boolean;
```
### printDrill {#printDrill--}
Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable.
```javascript
printDrill : boolean;
```
### altTextTitle {#altTextTitle--}
Gets and sets the title of the alter text.
```javascript
altTextTitle : string;
```
### altTextDescription {#altTextDescription--}
Gets the description of the alt text.
```javascript
altTextDescription : string;
```
### name {#name--}
Gets the name of the PivotTable
```javascript
name : string;
```
### columnHeaderCaption {#columnHeaderCaption--}
Gets the Column Header Caption of the PivotTable.
```javascript
columnHeaderCaption : string;
```
### indent {#indent--}
Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.
```javascript
indent : number;
```
### rowHeaderCaption {#rowHeaderCaption--}
Gets the Row Header Caption of the PivotTable.
```javascript
rowHeaderCaption : string;
```
### showRowHeaderCaption {#showRowHeaderCaption--}
Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs
```javascript
showRowHeaderCaption : boolean;
```
### customListSort {#customListSort--}
Indicates whether consider built-in custom list when sort data
```javascript
customListSort : boolean;
```
### pivotFormatConditions {#pivotFormatConditions--}
Readonly. Gets the Format Conditions of the pivot table.
```javascript
pivotFormatConditions : PivotFormatConditionCollection;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.ConditionalFormats property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### conditionalFormats {#conditionalFormats--}
Readonly. Gets the conditional formats of the pivot table.
```javascript
conditionalFormats : PivotConditionalFormatCollection;
```
### pageFieldOrder {#pageFieldOrder--}
Gets and sets the order in which page fields are added to the PivotTable report's layout.
```javascript
pageFieldOrder : PrintOrderType;
```
### pageFieldWrapCount {#pageFieldWrapCount--}
Gets the number of page fields in each column or row in the PivotTable report.
```javascript
pageFieldWrapCount : number;
```
### tag {#tag--}
Gets a string saved with the PivotTable report.
```javascript
tag : string;
```
### saveData {#saveData--}
Indicates whether data for the PivotTable report is saved with the workbook.
```javascript
saveData : boolean;
```
### refreshDataOnOpeningFile {#refreshDataOnOpeningFile--}
Indicates whether Refresh Data when Opening File.
```javascript
refreshDataOnOpeningFile : boolean;
```
### refreshDataFlag {#refreshDataFlag--}
Indicates whether Refreshing Data or not.
```javascript
refreshDataFlag : boolean;
```
**Remarks**
NOTE: This method is now obsolete. Instead, This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### sourceType {#sourceType--}
Readonly. Gets the data source type of the pivot table.
```javascript
sourceType : PivotTableSourceType;
```
### externalConnectionDataSource {#externalConnectionDataSource--}
Readonly. Gets the external connection data source.
```javascript
externalConnectionDataSource : ExternalConnection;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.GetSourceDataConnections() method. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### dataSource {#dataSource--}
Gets and sets the data source of the pivot table.
```javascript
dataSource : string[];
```
### pivotFormats {#pivotFormats--}
Readonly. Gets the collection of formats applied to PivotTable.
```javascript
pivotFormats : PivotTableFormatCollection;
```
### itemPrintTitles {#itemPrintTitles--}
Indicates whether PivotItem names should be repeated at the top of each printed page.
```javascript
itemPrintTitles : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.RepeatItemsOnEachPrintedPage property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### repeatItemsOnEachPrintedPage {#repeatItemsOnEachPrintedPage--}
Indicates whether pivot item captions on the row area are repeated on each printed page for pivot fields in tabular form.
```javascript
repeatItemsOnEachPrintedPage : boolean;
```
### printTitles {#printTitles--}
Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false.
```javascript
printTitles : boolean;
```
### displayImmediateItems {#displayImmediateItems--}
Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true.
```javascript
displayImmediateItems : boolean;
```
### isSelected {#isSelected--}
Indicates whether this PivotTable is selected.
```javascript
isSelected : boolean;
```
### showPivotStyleRowHeader {#showPivotStyleRowHeader--}
Indicates whether the row header in the pivot table should have the style applied.
```javascript
showPivotStyleRowHeader : boolean;
```
### showPivotStyleColumnHeader {#showPivotStyleColumnHeader--}
Indicates whether the column header in the pivot table should have the style applied.
```javascript
showPivotStyleColumnHeader : boolean;
```
### showPivotStyleRowStripes {#showPivotStyleRowStripes--}
Indicates whether row stripe formatting is applied.
```javascript
showPivotStyleRowStripes : boolean;
```
### showPivotStyleColumnStripes {#showPivotStyleColumnStripes--}
Indicates whether stripe formatting is applied for column.
```javascript
showPivotStyleColumnStripes : boolean;
```
### showPivotStyleLastColumn {#showPivotStyleLastColumn--}
Indicates whether the column formatting is applied.
```javascript
showPivotStyleLastColumn : boolean;
```
### isExcel2003Compatible() {#isExcel2003Compatible--}
```javascript
isExcel2003Compatible() : boolean;
```
### setIsExcel2003Compatible(boolean) {#setIsExcel2003Compatible-boolean-}
```javascript
setIsExcel2003Compatible(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRefreshedByWho() {#getRefreshedByWho--}
```javascript
getRefreshedByWho() : string;
```
### getRefreshDate() {#getRefreshDate--}
```javascript
getRefreshDate() : Date;
```
### getPivotTableStyleName() {#getPivotTableStyleName--}
```javascript
getPivotTableStyleName() : string;
```
### setPivotTableStyleName(string) {#setPivotTableStyleName-string-}
```javascript
setPivotTableStyleName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getPivotTableStyleType() {#getPivotTableStyleType--}
```javascript
getPivotTableStyleType() : PivotTableStyleType;
```
**Returns**
[PivotTableStyleType](../pivottablestyletype/)
### setPivotTableStyleType(PivotTableStyleType) {#setPivotTableStyleType-pivottablestyletype-}
```javascript
setPivotTableStyleType(value: PivotTableStyleType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotTableStyleType](../pivottablestyletype/) | The value to set. |
### getColumnFields() {#getColumnFields--}
```javascript
getColumnFields() : PivotFieldCollection;
```
**Returns**
[PivotFieldCollection](../pivotfieldcollection/)
### getRowFields() {#getRowFields--}
```javascript
getRowFields() : PivotFieldCollection;
```
**Returns**
[PivotFieldCollection](../pivotfieldcollection/)
### getPageFields() {#getPageFields--}
```javascript
getPageFields() : PivotFieldCollection;
```
**Returns**
[PivotFieldCollection](../pivotfieldcollection/)
### getDataFields() {#getDataFields--}
```javascript
getDataFields() : PivotFieldCollection;
```
**Returns**
[PivotFieldCollection](../pivotfieldcollection/)
### getDataField() {#getDataField--}
```javascript
getDataField() : PivotField;
```
**Returns**
[PivotField](../pivotfield/)
### getBaseFields() {#getBaseFields--}
```javascript
getBaseFields() : PivotFieldCollection;
```
**Returns**
[PivotFieldCollection](../pivotfieldcollection/)
### getPivotFilters() {#getPivotFilters--}
```javascript
getPivotFilters() : PivotFilterCollection;
```
**Returns**
[PivotFilterCollection](../pivotfiltercollection/)
### getColumnRange() {#getColumnRange--}
```javascript
getColumnRange() : CellArea;
```
**Returns**
[CellArea](../cellarea/)
### getRowRange() {#getRowRange--}
```javascript
getRowRange() : CellArea;
```
**Returns**
[CellArea](../cellarea/)
### getDataBodyRange() {#getDataBodyRange--}
```javascript
getDataBodyRange() : CellArea;
```
**Returns**
[CellArea](../cellarea/)
### getTableRange1() {#getTableRange1--}
```javascript
getTableRange1() : CellArea;
```
**Returns**
[CellArea](../cellarea/)
### getTableRange2() {#getTableRange2--}
```javascript
getTableRange2() : CellArea;
```
**Returns**
[CellArea](../cellarea/)
### isGridDropZones() {#isGridDropZones--}
```javascript
isGridDropZones() : boolean;
```
### setIsGridDropZones(boolean) {#setIsGridDropZones-boolean-}
```javascript
setIsGridDropZones(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```javascript
getShowColumnGrandTotals() : boolean;
```
### setShowColumnGrandTotals(boolean) {#setShowColumnGrandTotals-boolean-}
```javascript
setShowColumnGrandTotals(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```javascript
getShowRowGrandTotals() : boolean;
```
### setShowRowGrandTotals(boolean) {#setShowRowGrandTotals-boolean-}
```javascript
setShowRowGrandTotals(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getColumnGrand() {#getColumnGrand--}
```javascript
getColumnGrand() : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.ShowColumnGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### setColumnGrand(boolean) {#setColumnGrand-boolean-}
```javascript
setColumnGrand(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.ShowColumnGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### getRowGrand() {#getRowGrand--}
```javascript
getRowGrand() : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.ShowRowGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### setRowGrand(boolean) {#setRowGrand-boolean-}
```javascript
setRowGrand(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.ShowRowGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### getDisplayNullString() {#getDisplayNullString--}
```javascript
getDisplayNullString() : boolean;
```
### setDisplayNullString(boolean) {#setDisplayNullString-boolean-}
```javascript
setDisplayNullString(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getNullString() {#getNullString--}
```javascript
getNullString() : string;
```
### setNullString(string) {#setNullString-string-}
```javascript
setNullString(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getDisplayErrorString() {#getDisplayErrorString--}
```javascript
getDisplayErrorString() : boolean;
```
### setDisplayErrorString(boolean) {#setDisplayErrorString-boolean-}
```javascript
setDisplayErrorString(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```javascript
getDataFieldHeaderName() : string;
```
### setDataFieldHeaderName(string) {#setDataFieldHeaderName-string-}
```javascript
setDataFieldHeaderName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getErrorString() {#getErrorString--}
```javascript
getErrorString() : string;
```
### setErrorString(string) {#setErrorString-string-}
```javascript
setErrorString(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isAutoFormat() {#isAutoFormat--}
```javascript
isAutoFormat() : boolean;
```
### setIsAutoFormat(boolean) {#setIsAutoFormat-boolean-}
```javascript
setIsAutoFormat(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```javascript
getAutofitColumnWidthOnUpdate() : boolean;
```
### setAutofitColumnWidthOnUpdate(boolean) {#setAutofitColumnWidthOnUpdate-boolean-}
```javascript
setAutofitColumnWidthOnUpdate(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAutoFormatType() {#getAutoFormatType--}
```javascript
getAutoFormatType() : PivotTableAutoFormatType;
```
**Returns**
[PivotTableAutoFormatType](../pivottableautoformattype/)
### setAutoFormatType(PivotTableAutoFormatType) {#setAutoFormatType-pivottableautoformattype-}
```javascript
setAutoFormatType(value: PivotTableAutoFormatType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotTableAutoFormatType](../pivottableautoformattype/) | The value to set. |
### getHasBlankRows() {#getHasBlankRows--}
```javascript
getHasBlankRows() : boolean;
```
### setHasBlankRows(boolean) {#setHasBlankRows-boolean-}
```javascript
setHasBlankRows(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getMergeLabels() {#getMergeLabels--}
```javascript
getMergeLabels() : boolean;
```
### setMergeLabels(boolean) {#setMergeLabels-boolean-}
```javascript
setMergeLabels(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPreserveFormatting() {#getPreserveFormatting--}
```javascript
getPreserveFormatting() : boolean;
```
### setPreserveFormatting(boolean) {#setPreserveFormatting-boolean-}
```javascript
setPreserveFormatting(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowDrill() {#getShowDrill--}
```javascript
getShowDrill() : boolean;
```
### setShowDrill(boolean) {#setShowDrill-boolean-}
```javascript
setShowDrill(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getEnableDrilldown() {#getEnableDrilldown--}
```javascript
getEnableDrilldown() : boolean;
```
### setEnableDrilldown(boolean) {#setEnableDrilldown-boolean-}
```javascript
setEnableDrilldown(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getEnableFieldDialog() {#getEnableFieldDialog--}
```javascript
getEnableFieldDialog() : boolean;
```
### setEnableFieldDialog(boolean) {#setEnableFieldDialog-boolean-}
```javascript
setEnableFieldDialog(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getEnableFieldList() {#getEnableFieldList--}
```javascript
getEnableFieldList() : boolean;
```
### setEnableFieldList(boolean) {#setEnableFieldList-boolean-}
```javascript
setEnableFieldList(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getEnableWizard() {#getEnableWizard--}
```javascript
getEnableWizard() : boolean;
```
### setEnableWizard(boolean) {#setEnableWizard-boolean-}
```javascript
setEnableWizard(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```javascript
getSubtotalHiddenPageItems() : boolean;
```
### setSubtotalHiddenPageItems(boolean) {#setSubtotalHiddenPageItems-boolean-}
```javascript
setSubtotalHiddenPageItems(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getGrandTotalName() {#getGrandTotalName--}
```javascript
getGrandTotalName() : string;
```
### setGrandTotalName(string) {#setGrandTotalName-string-}
```javascript
setGrandTotalName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getManualUpdate() {#getManualUpdate--}
```javascript
getManualUpdate() : boolean;
```
### setManualUpdate(boolean) {#setManualUpdate-boolean-}
```javascript
setManualUpdate(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```javascript
isMultipleFieldFilters() : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.AllowMultipleFiltersPerField property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### setIsMultipleFieldFilters(boolean) {#setIsMultipleFieldFilters-boolean-}
```javascript
setIsMultipleFieldFilters(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.AllowMultipleFiltersPerField property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```javascript
getAllowMultipleFiltersPerField() : boolean;
```
### setAllowMultipleFiltersPerField(boolean) {#setAllowMultipleFiltersPerField-boolean-}
```javascript
setAllowMultipleFiltersPerField(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getMissingItemsLimit() {#getMissingItemsLimit--}
```javascript
getMissingItemsLimit() : PivotMissingItemLimitType;
```
**Returns**
[PivotMissingItemLimitType](../pivotmissingitemlimittype/)
### setMissingItemsLimit(PivotMissingItemLimitType) {#setMissingItemsLimit-pivotmissingitemlimittype-}
```javascript
setMissingItemsLimit(value: PivotMissingItemLimitType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotMissingItemLimitType](../pivotmissingitemlimittype/) | The value to set. |
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```javascript
getEnableDataValueEditing() : boolean;
```
### setEnableDataValueEditing(boolean) {#setEnableDataValueEditing-boolean-}
```javascript
setEnableDataValueEditing(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowDataTips() {#getShowDataTips--}
```javascript
getShowDataTips() : boolean;
```
### setShowDataTips(boolean) {#setShowDataTips-boolean-}
```javascript
setShowDataTips(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```javascript
getShowMemberPropertyTips() : boolean;
```
### setShowMemberPropertyTips(boolean) {#setShowMemberPropertyTips-boolean-}
```javascript
setShowMemberPropertyTips(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowValuesRow() {#getShowValuesRow--}
```javascript
getShowValuesRow() : boolean;
```
### setShowValuesRow(boolean) {#setShowValuesRow-boolean-}
```javascript
setShowValuesRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowEmptyCol() {#getShowEmptyCol--}
```javascript
getShowEmptyCol() : boolean;
```
### setShowEmptyCol(boolean) {#setShowEmptyCol-boolean-}
```javascript
setShowEmptyCol(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowEmptyRow() {#getShowEmptyRow--}
```javascript
getShowEmptyRow() : boolean;
```
### setShowEmptyRow(boolean) {#setShowEmptyRow-boolean-}
```javascript
setShowEmptyRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFieldListSortAscending() {#getFieldListSortAscending--}
```javascript
getFieldListSortAscending() : boolean;
```
### setFieldListSortAscending(boolean) {#setFieldListSortAscending-boolean-}
```javascript
setFieldListSortAscending(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPrintDrill() {#getPrintDrill--}
```javascript
getPrintDrill() : boolean;
```
### setPrintDrill(boolean) {#setPrintDrill-boolean-}
```javascript
setPrintDrill(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAltTextTitle() {#getAltTextTitle--}
```javascript
getAltTextTitle() : string;
```
### setAltTextTitle(string) {#setAltTextTitle-string-}
```javascript
setAltTextTitle(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getAltTextDescription() {#getAltTextDescription--}
```javascript
getAltTextDescription() : string;
```
### setAltTextDescription(string) {#setAltTextDescription-string-}
```javascript
setAltTextDescription(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getName() {#getName--}
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```javascript
getColumnHeaderCaption() : string;
```
### setColumnHeaderCaption(string) {#setColumnHeaderCaption-string-}
```javascript
setColumnHeaderCaption(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getIndent() {#getIndent--}
```javascript
getIndent() : number;
```
### setIndent(number) {#setIndent-number-}
```javascript
setIndent(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRowHeaderCaption() {#getRowHeaderCaption--}
```javascript
getRowHeaderCaption() : string;
```
### setRowHeaderCaption(string) {#setRowHeaderCaption-string-}
```javascript
setRowHeaderCaption(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```javascript
getShowRowHeaderCaption() : boolean;
```
### setShowRowHeaderCaption(boolean) {#setShowRowHeaderCaption-boolean-}
```javascript
setShowRowHeaderCaption(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCustomListSort() {#getCustomListSort--}
```javascript
getCustomListSort() : boolean;
```
### setCustomListSort(boolean) {#setCustomListSort-boolean-}
```javascript
setCustomListSort(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPivotFormatConditions() {#getPivotFormatConditions--}
```javascript
getPivotFormatConditions() : PivotFormatConditionCollection;
```
**Returns**
[PivotFormatConditionCollection](../pivotformatconditioncollection/)
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.ConditionalFormats property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### getConditionalFormats() {#getConditionalFormats--}
```javascript
getConditionalFormats() : PivotConditionalFormatCollection;
```
**Returns**
[PivotConditionalFormatCollection](../pivotconditionalformatcollection/)
### getPageFieldOrder() {#getPageFieldOrder--}
```javascript
getPageFieldOrder() : PrintOrderType;
```
**Returns**
[PrintOrderType](../printordertype/)
### setPageFieldOrder(PrintOrderType) {#setPageFieldOrder-printordertype-}
```javascript
setPageFieldOrder(value: PrintOrderType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintOrderType](../printordertype/) | The value to set. |
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```javascript
getPageFieldWrapCount() : number;
```
### setPageFieldWrapCount(number) {#setPageFieldWrapCount-number-}
```javascript
setPageFieldWrapCount(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getTag() {#getTag--}
```javascript
getTag() : string;
```
### setTag(string) {#setTag-string-}
```javascript
setTag(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getSaveData() {#getSaveData--}
```javascript
getSaveData() : boolean;
```
### setSaveData(boolean) {#setSaveData-boolean-}
```javascript
setSaveData(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```javascript
getRefreshDataOnOpeningFile() : boolean;
```
### setRefreshDataOnOpeningFile(boolean) {#setRefreshDataOnOpeningFile-boolean-}
```javascript
setRefreshDataOnOpeningFile(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRefreshDataFlag() {#getRefreshDataFlag--}
```javascript
getRefreshDataFlag() : boolean;
```
**Remarks**
NOTE: This method is now obsolete. Instead, This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### setRefreshDataFlag(boolean) {#setRefreshDataFlag-boolean-}
```javascript
setRefreshDataFlag(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
NOTE: This method is now obsolete. Instead, This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### getSourceType() {#getSourceType--}
```javascript
getSourceType() : PivotTableSourceType;
```
**Returns**
[PivotTableSourceType](../pivottablesourcetype/)
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```javascript
getExternalConnectionDataSource() : ExternalConnection;
```
**Returns**
[ExternalConnection](../externalconnection/)
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.GetSourceDataConnections() method. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### getDataSource() {#getDataSource--}
```javascript
getDataSource() : string[];
```
**Returns**
string[]
### setDataSource(string[]) {#setDataSource-stringarray-}
```javascript
setDataSource(value: string[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string[] | The value to set. |
### getPivotFormats() {#getPivotFormats--}
```javascript
getPivotFormats() : PivotTableFormatCollection;
```
**Returns**
[PivotTableFormatCollection](../pivottableformatcollection/)
### getItemPrintTitles() {#getItemPrintTitles--}
```javascript
getItemPrintTitles() : boolean;
```
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.RepeatItemsOnEachPrintedPage property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### setItemPrintTitles(boolean) {#setItemPrintTitles-boolean-}
```javascript
setItemPrintTitles(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.RepeatItemsOnEachPrintedPage property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```javascript
getRepeatItemsOnEachPrintedPage() : boolean;
```
### setRepeatItemsOnEachPrintedPage(boolean) {#setRepeatItemsOnEachPrintedPage-boolean-}
```javascript
setRepeatItemsOnEachPrintedPage(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPrintTitles() {#getPrintTitles--}
```javascript
getPrintTitles() : boolean;
```
### setPrintTitles(boolean) {#setPrintTitles-boolean-}
```javascript
setPrintTitles(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```javascript
getDisplayImmediateItems() : boolean;
```
### setDisplayImmediateItems(boolean) {#setDisplayImmediateItems-boolean-}
```javascript
setDisplayImmediateItems(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isSelected() {#isSelected--}
```javascript
isSelected() : boolean;
```
### setIsSelected(boolean) {#setIsSelected-boolean-}
```javascript
setIsSelected(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```javascript
getShowPivotStyleRowHeader() : boolean;
```
### setShowPivotStyleRowHeader(boolean) {#setShowPivotStyleRowHeader-boolean-}
```javascript
setShowPivotStyleRowHeader(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```javascript
getShowPivotStyleColumnHeader() : boolean;
```
### setShowPivotStyleColumnHeader(boolean) {#setShowPivotStyleColumnHeader-boolean-}
```javascript
setShowPivotStyleColumnHeader(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```javascript
getShowPivotStyleRowStripes() : boolean;
```
### setShowPivotStyleRowStripes(boolean) {#setShowPivotStyleRowStripes-boolean-}
```javascript
setShowPivotStyleRowStripes(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```javascript
getShowPivotStyleColumnStripes() : boolean;
```
### setShowPivotStyleColumnStripes(boolean) {#setShowPivotStyleColumnStripes-boolean-}
```javascript
setShowPivotStyleColumnStripes(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```javascript
getShowPivotStyleLastColumn() : boolean;
```
### setShowPivotStyleLastColumn(boolean) {#setShowPivotStyleLastColumn-boolean-}
```javascript
setShowPivotStyleLastColumn(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### dispose() {#dispose--}
Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.
```javascript
dispose() : void;
```
### copyStyle(PivotTable) {#copyStyle-pivottable-}
Copies named style from another pivot table.
```javascript
copyStyle(pivotTable: PivotTable) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../pivottable/) | Source pivot table. |
### showReportFilterPage(PivotField) {#showReportFilterPage-pivotfield-}
Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields.
```javascript
showReportFilterPage(pageField: PivotField) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageField | [PivotField](../pivotfield/) | The PivotField object |
### showReportFilterPageByName(string) {#showReportFilterPageByName-string-}
Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields.
```javascript
showReportFilterPageByName(fieldName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | string | The name of PivotField |
### showReportFilterPageByIndex(number) {#showReportFilterPageByIndex-number-}
Show all the report filter pages according to the position index in the PageFields
```javascript
showReportFilterPageByIndex(posIndex: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| posIndex | number | The position index in the PageFields |
### removeField(PivotFieldType, string) {#removeField-pivotfieldtype-string-}
Removes a field from specific field area
```javascript
removeField(fieldType: PivotFieldType, fieldName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | [PivotFieldType](../pivotfieldtype/) | The fields area type. |
| fieldName | string | The name in the base fields. |
### removeField(PivotFieldType, number) {#removeField-pivotfieldtype-number-}
Removes a field from specific field area
```javascript
removeField(fieldType: PivotFieldType, baseFieldIndex: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | [PivotFieldType](../pivotfieldtype/) | The fields area type. |
| baseFieldIndex | number | The field index in the base fields. |
### removeField(PivotFieldType, PivotField) {#removeField-pivotfieldtype-pivotfield-}
Remove field from specific field area
```javascript
removeField(fieldType: PivotFieldType, pivotField: PivotField) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | [PivotFieldType](../pivotfieldtype/) | the fields area type. |
| pivotField | [PivotField](../pivotfield/) | the field in the base fields. |
### addFieldToArea(PivotFieldType, string) {#addFieldToArea-pivotfieldtype-string-}
Adds the field to the specific area.
```javascript
addFieldToArea(fieldType: PivotFieldType, fieldName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | [PivotFieldType](../pivotfieldtype/) | The fields area type. |
| fieldName | string | The name in the base fields. |
**Returns**
The field position in the specific fields.If there is no field named as it, return -1.
### addFieldToArea(PivotFieldType, number) {#addFieldToArea-pivotfieldtype-number-}
Adds the field to the specific area.
```javascript
addFieldToArea(fieldType: PivotFieldType, baseFieldIndex: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | [PivotFieldType](../pivotfieldtype/) | The fields area type. |
| baseFieldIndex | number | The field index in the base fields. |
**Returns**
The field position in the specific fields.
### addFieldToArea(PivotFieldType, PivotField) {#addFieldToArea-pivotfieldtype-pivotfield-}
Adds the field to the specific area.
```javascript
addFieldToArea(fieldType: PivotFieldType, pivotField: PivotField) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | [PivotFieldType](../pivotfieldtype/) | the fields area type. |
| pivotField | [PivotField](../pivotfield/) | the field in the base fields. |
**Returns**
the field position in the specific fields.
### addCalculatedField(string, string, boolean) {#addCalculatedField-string-string-boolean-}
Adds a calculated field to pivot field.
```javascript
addCalculatedField(name: string, formula: string, dragToDataArea: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the calculated field |
| formula | string | The formula of the calculated field. |
| dragToDataArea | boolean | True,drag this field to data area immediately |
### addCalculatedField(string, string) {#addCalculatedField-string-string-}
Adds a calculated field to pivot field and drag it to data area.
```javascript
addCalculatedField(name: string, formula: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the calculated field |
| formula | string | The formula of the calculated field. |
### getFields(PivotFieldType) {#getFields-pivotfieldtype-}
Gets the specific pivot field list by the region.
```javascript
getFields(fieldType: PivotFieldType) : PivotFieldCollection;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | [PivotFieldType](../pivotfieldtype/) | the region type. |
**Returns**
the specific pivot field collection
### move(number, number) {#move-number-number-}
Moves the PivotTable to a different location in the worksheet.
```javascript
move(row: number, column: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | row index. |
| column | number | column index. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.MoveTo() method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### move(string) {#move-string-}
Moves the PivotTable to a different location in the worksheet.
```javascript
move(destCellName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destCellName | string | the dest cell name. |
**Remarks**
NOTE: This property is now obsolete. Instead, please use PivotTable.MoveTo() method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### moveTo(number, number) {#moveTo-number-number-}
Moves the PivotTable to a different location in the worksheet.
```javascript
moveTo(row: number, column: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | row index. |
| column | number | column index. |
### moveTo(string) {#moveTo-string-}
Moves the PivotTable to a different location in the worksheet.
```javascript
moveTo(destCellName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destCellName | string | the dest cell name. |
### getSourceDataConnections() {#getSourceDataConnections--}
Gets the external connection data sources.
```javascript
getSourceDataConnections() : ExternalConnection[];
```
**Returns**
[ExternalConnection](../externalconnection/)[]
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
Gets the name of external source data connections.
```javascript
getNamesOfSourceDataConnections() : string[];
```
**Returns**
string[]
### changeDataSource(string[]) {#changeDataSource-stringarray-}
Set pivottable's source data.
```javascript
changeDataSource(source: string[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | string[] |  |
### getSource() {#getSource--}
Get pivottable's source data.
```javascript
getSource() : string[];
```
**Returns**
string[]
### getSource(boolean) {#getSource-boolean-}
Get pivottable's source data.
```javascript
getSource(isOriginal: boolean) : string[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isOriginal | boolean | Indicates whether to return original or display data source |
**Returns**
string[]
### refreshData() {#refreshData--}
Refreshes pivottable's data and setting from it's data source.
```javascript
refreshData() : PivotRefreshState;
```
**Returns**
[PivotRefreshState](../pivotrefreshstate/)
**Remarks**
We will gather data from data source to a pivot cache ,then calculate the data in the cache to the cells. This method is only used to gather all data to a pivot cache.
### refreshData(PivotTableRefreshOption) {#refreshData-pivottablerefreshoption-}
Refreshes pivottable's data and setting from it's data source with options.
```javascript
refreshData(option: PivotTableRefreshOption) : PivotRefreshState;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../pivottablerefreshoption/) | The options for refreshing data source of pivot table. |
**Returns**
[PivotRefreshState](../pivotrefreshstate/)
### calculateData() {#calculateData--}
Calculates pivottable's data to cells.
```javascript
calculateData() : void;
```
**Remarks**
Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.
### calculateData(PivotTableCalculateOption) {#calculateData-pivottablecalculateoption-}
Calculating pivot tables with options
```javascript
calculateData(option: PivotTableCalculateOption) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../pivottablecalculateoption/) |  |
### clearData() {#clearData--}
Clear PivotTable's data and formatting
```javascript
clearData() : void;
```
**Remarks**
If this method is not called before you add or delete PivotField, Maybe the PivotTable data is not corrected
### calculateRange() {#calculateRange--}
Calculates pivottable's range.
```javascript
calculateRange() : void;
```
**Remarks**
If this method is not been called,maybe the pivottable range is not corrected.
### formatAll(Style) {#formatAll-style-}
Format all the cell in the pivottable area
```javascript
formatAll(style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | Style which is to format |
### formatRow(number, Style) {#formatRow-number-style-}
Format the row data in the pivottable area
```javascript
formatRow(row: number, style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row Index of the Row object |
| style | [Style](../style/) | Style which is to format |
### format(PivotArea, Style) {#format-pivotarea-style-}
Formats selected area of the PivotTable.
```javascript
format(pivotArea: PivotArea, style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | [PivotArea](../pivotarea/) | The selected pivot view area. |
| style | [Style](../style/) | The formatted setting. |
### format(CellArea, Style) {#format-cellarea-style-}
Formats selected area of the PivotTable.
```javascript
format(ca: CellArea, style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The range of the cells. |
| style | [Style](../style/) | The style |
### format(number, number, Style) {#format-number-number-style-}
Format the cell in the pivottable area
```javascript
format(row: number, column: number, style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row Index of the cell |
| column | number | Column index of the cell |
| style | [Style](../style/) | Style which is to format the cell |
### selectArea(CellArea) {#selectArea-cellarea-}
Select an area of pivot table view.
```javascript
selectArea(ca: CellArea) : PivotAreaCollection;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The cell area. |
**Returns**
[PivotAreaCollection](../pivotareacollection/)
### showDetail(number, number, boolean, number, number) {#showDetail-number-number-boolean-number-number-}
Show the detail of one item in the data region to a new Table.
```javascript
showDetail(rowOffset: number, columnOffset: number, newSheet: boolean, destRow: number, destColumn: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | Offset to the first data row in the data region. |
| columnOffset | number | Offset to the first data column in the data region. |
| newSheet | boolean | Show the detail to a new worksheet. |
| destRow | number | The target row. |
| destColumn | number | The target column. |
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
Gets horizontal page breaks of this pivot table.
```javascript
getHorizontalPageBreaks() : number[];
```
**Returns**
number[]
### showInCompactForm() {#showInCompactForm--}
Layouts the PivotTable in compact form.
```javascript
showInCompactForm() : void;
```
### showInOutlineForm() {#showInOutlineForm--}
Layouts the PivotTable in outline form.
```javascript
showInOutlineForm() : void;
```
### showInTabularForm() {#showInTabularForm--}
Layouts the PivotTable in tabular form.
```javascript
showInTabularForm() : void;
```
### getCellByDisplayName(string) {#getCellByDisplayName-string-}
Gets the [Cell](../cell/) object by the display name of PivotField.
```javascript
getCellByDisplayName(displayName: string) : Cell;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| displayName | string | the DisplayName of PivotField |
**Returns**
the Cell object
### getChildren() {#getChildren--}
Gets the Children Pivot Tables which use this PivotTable data as data source.
```javascript
getChildren() : PivotTable[];
```
**Returns**
the PivotTable array object
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
