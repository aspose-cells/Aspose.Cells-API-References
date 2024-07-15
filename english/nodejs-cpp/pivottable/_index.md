---
title: PivotTable
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Summary description for PivotTable.
type: docs
url: /nodejs-cpp/pivottable/
---

## PivotTable class

Summary description for PivotTable.

```javascript
class PivotTable;
```


## Methods

| Method | Description |
| --- | --- |
| [isExcel2003Compatible()](#isExcel2003Compatible--)| Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true. |
| [setIsExcel2003Compatible(boolean)](#setIsExcel2003Compatible-boolean-)| Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true. |
| [getRefreshedByWho()](#getRefreshedByWho--)| Gets the name of the last user who refreshed this PivotTable |
| [getRefreshDate()](#getRefreshDate--)| Gets the last date time when the PivotTable was refreshed. |
| [getPivotTableStyleName()](#getPivotTableStyleName--)| Gets and sets the pivottable style name. |
| [setPivotTableStyleName(string)](#setPivotTableStyleName-string-)| Gets and sets the pivottable style name. |
| [getPivotTableStyleType()](#getPivotTableStyleType--)| Gets and sets the built-in pivot table style. |
| [setPivotTableStyleType(PivotTableStyleType)](#setPivotTableStyleType-pivottablestyletype-)| Gets and sets the built-in pivot table style. |
| [getColumnFields()](#getColumnFields--)| Returns a PivotFields object that are currently shown as column fields. |
| [getRowFields()](#getRowFields--)| Returns a PivotFields object that are currently shown as row fields. |
| [getPageFields()](#getPageFields--)| Returns a PivotFields object that are currently shown as page fields. |
| [getDataFields()](#getDataFields--)| Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area. |
| [getDataField()](#getDataField--)| Gets a [PivotField](../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method . |
| [getBaseFields()](#getBaseFields--)| Returns all base pivot fields in the PivotTable. |
| [getPivotFilters()](#getPivotFilters--)| Returns a list of pivot filters. |
| [getColumnRange()](#getColumnRange--)| Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only. |
| [getRowRange()](#getRowRange--)| Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only. |
| [getDataBodyRange()](#getDataBodyRange--)| Returns a [CellArea](../cellarea/) object that represents the range that contains the data area in the list between the header row and the insert row. Read-only. |
| [getTableRange1()](#getTableRange1--)| Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only. |
| [getTableRange2()](#getTableRange2--)| Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only. |
| [getColumnGrand()](#getColumnGrand--)| Indicates whether the PivotTable report shows grand totals for columns. |
| [setColumnGrand(boolean)](#setColumnGrand-boolean-)| Indicates whether the PivotTable report shows grand totals for columns. |
| [isGridDropZones()](#isGridDropZones--)| Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid) |
| [setIsGridDropZones(boolean)](#setIsGridDropZones-boolean-)| Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid) |
| [getRowGrand()](#getRowGrand--)| Indicates whether the PivotTable report shows grand totals for rows. |
| [setRowGrand(boolean)](#setRowGrand-boolean-)| Indicates whether the PivotTable report shows grand totals for rows. |
| [getDisplayNullString()](#getDisplayNullString--)| Indicates whether the PivotTable report displays a custom string if the value is null. |
| [setDisplayNullString(boolean)](#setDisplayNullString-boolean-)| Indicates whether the PivotTable report displays a custom string if the value is null. |
| [getNullString()](#getNullString--)| Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [setNullString(string)](#setNullString-string-)| Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string. |
| [getDisplayErrorString()](#getDisplayErrorString--)| Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [setDisplayErrorString(boolean)](#setDisplayErrorString-boolean-)| Indicates whether the PivotTable report displays a custom string in cells that contain errors. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--)| Gets and sets the name of the value area field header in the PivotTable. |
| [setDataFieldHeaderName(string)](#setDataFieldHeaderName-string-)| Gets and sets the name of the value area field header in the PivotTable. |
| [getErrorString()](#getErrorString--)| Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [setErrorString(string)](#setErrorString-string-)| Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string. |
| [isAutoFormat()](#isAutoFormat--)| Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003 |
| [setIsAutoFormat(boolean)](#setIsAutoFormat-boolean-)| Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003 |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--)| Indicates whether autofitting column width on update |
| [setAutofitColumnWidthOnUpdate(boolean)](#setAutofitColumnWidthOnUpdate-boolean-)| Indicates whether autofitting column width on update |
| [getAutoFormatType()](#getAutoFormatType--)| Gets and sets the auto format type of PivotTable. |
| [setAutoFormatType(PivotTableAutoFormatType)](#setAutoFormatType-pivottableautoformattype-)| Gets and sets the auto format type of PivotTable. |
| [getHasBlankRows()](#getHasBlankRows--)| Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows. |
| [setHasBlankRows(boolean)](#setHasBlankRows-boolean-)| Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows. |
| [getMergeLabels()](#getMergeLabels--)| True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [setMergeLabels(boolean)](#setMergeLabels-boolean-)| True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells. |
| [getPreserveFormatting()](#getPreserveFormatting--)| Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [setPreserveFormatting(boolean)](#setPreserveFormatting-boolean-)| Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated. |
| [getShowDrill()](#getShowDrill--)| Gets and sets whether showing expand/collapse buttons. |
| [setShowDrill(boolean)](#setShowDrill-boolean-)| Gets and sets whether showing expand/collapse buttons. |
| [getEnableDrilldown()](#getEnableDrilldown--)| Gets whether drilldown is enabled. |
| [setEnableDrilldown(boolean)](#setEnableDrilldown-boolean-)| Gets whether drilldown is enabled. |
| [getEnableFieldDialog()](#getEnableFieldDialog--)| Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [setEnableFieldDialog(boolean)](#setEnableFieldDialog-boolean-)| Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field. |
| [getEnableFieldList()](#getEnableFieldList--)| Gets whether enable the field list for the PivotTable. |
| [setEnableFieldList(boolean)](#setEnableFieldList-boolean-)| Gets whether enable the field list for the PivotTable. |
| [getEnableWizard()](#getEnableWizard--)| Indicates whether the PivotTable Wizard is available. |
| [setEnableWizard(boolean)](#setEnableWizard-boolean-)| Indicates whether the PivotTable Wizard is available. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--)| Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False. |
| [setSubtotalHiddenPageItems(boolean)](#setSubtotalHiddenPageItems-boolean-)| Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False. |
| [getGrandTotalName()](#getGrandTotalName--)| Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total". |
| [setGrandTotalName(string)](#setGrandTotalName-string-)| Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total". |
| [getManualUpdate()](#getManualUpdate--)| Indicates whether the PivotTable report is recalculated only at the user's request. |
| [setManualUpdate(boolean)](#setManualUpdate-boolean-)| Indicates whether the PivotTable report is recalculated only at the user's request. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--)| Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [setIsMultipleFieldFilters(boolean)](#setIsMultipleFieldFilters-boolean-)| Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [getMissingItemsLimit()](#getMissingItemsLimit--)| Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [setMissingItemsLimit(PivotMissingItemLimitType)](#setMissingItemsLimit-pivotmissingitemlimittype-)| Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--)| Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area |
| [setEnableDataValueEditing(boolean)](#setEnableDataValueEditing-boolean-)| Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area |
| [getShowDataTips()](#getShowDataTips--)| Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [setShowDataTips(boolean)](#setShowDataTips-boolean-)| Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--)| Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [setShowMemberPropertyTips(boolean)](#setShowMemberPropertyTips-boolean-)| Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips. |
| [getShowValuesRow()](#getShowValuesRow--)| Specifies a boolean value that indicates whether show values row. show the values row |
| [setShowValuesRow(boolean)](#setShowValuesRow-boolean-)| Specifies a boolean value that indicates whether show values row. show the values row |
| [getShowEmptyCol()](#getShowEmptyCol--)| Specifies a boolean value that indicates whether to include empty columns in the table |
| [setShowEmptyCol(boolean)](#setShowEmptyCol-boolean-)| Specifies a boolean value that indicates whether to include empty columns in the table |
| [getShowEmptyRow()](#getShowEmptyRow--)| Specifies a boolean value that indicates whether to include empty rows in the table. |
| [setShowEmptyRow(boolean)](#setShowEmptyRow-boolean-)| Specifies a boolean value that indicates whether to include empty rows in the table. |
| [getFieldListSortAscending()](#getFieldListSortAscending--)| Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [setFieldListSortAscending(boolean)](#setFieldListSortAscending-boolean-)| Indicates whether fields in the PivotTable are sorted in non-default order in the field list. |
| [getPrintDrill()](#getPrintDrill--)| Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable. |
| [setPrintDrill(boolean)](#setPrintDrill-boolean-)| Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable. |
| [getAltTextTitle()](#getAltTextTitle--)| Gets the title of the altertext |
| [setAltTextTitle(string)](#setAltTextTitle-string-)| Gets the title of the altertext |
| [getAltTextDescription()](#getAltTextDescription--)| Gets the description of the alt text |
| [setAltTextDescription(string)](#setAltTextDescription-string-)| Gets the description of the alt text |
| [getName()](#getName--)| Gets the name of the PivotTable |
| [setName(string)](#setName-string-)| Gets the name of the PivotTable |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--)| Gets the Column Header Caption of the PivotTable. |
| [setColumnHeaderCaption(string)](#setColumnHeaderCaption-string-)| Gets the Column Header Caption of the PivotTable. |
| [getIndent()](#getIndent--)| Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [setIndent(number)](#setIndent-number-)| Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [getRowHeaderCaption()](#getRowHeaderCaption--)| Gets the Row Header Caption of the PivotTable. |
| [setRowHeaderCaption(string)](#setRowHeaderCaption-string-)| Gets the Row Header Caption of the PivotTable. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--)| Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs |
| [setShowRowHeaderCaption(boolean)](#setShowRowHeaderCaption-boolean-)| Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs |
| [getCustomListSort()](#getCustomListSort--)| Indicates whether consider built-in custom list when sort data |
| [setCustomListSort(boolean)](#setCustomListSort-boolean-)| Indicates whether consider built-in custom list when sort data |
| [getPivotFormatConditions()](#getPivotFormatConditions--)| Gets the Format Conditions of the pivot table. |
| [getPageFieldOrder()](#getPageFieldOrder--)| Gets the order in which page fields are added to the PivotTable report's layout. |
| [setPageFieldOrder(PrintOrderType)](#setPageFieldOrder-printordertype-)| Gets the order in which page fields are added to the PivotTable report's layout. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--)| Gets the number of page fields in each column or row in the PivotTable report. |
| [setPageFieldWrapCount(number)](#setPageFieldWrapCount-number-)| Gets the number of page fields in each column or row in the PivotTable report. |
| [getTag()](#getTag--)| Gets a string saved with the PivotTable report. |
| [setTag(string)](#setTag-string-)| Gets a string saved with the PivotTable report. |
| [getSaveData()](#getSaveData--)| Indicates whether data for the PivotTable report is saved with the workbook. |
| [setSaveData(boolean)](#setSaveData-boolean-)| Indicates whether data for the PivotTable report is saved with the workbook. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--)| Indicates whether Refresh Data when Opening File. |
| [setRefreshDataOnOpeningFile(boolean)](#setRefreshDataOnOpeningFile-boolean-)| Indicates whether Refresh Data when Opening File. |
| [getRefreshDataFlag()](#getRefreshDataFlag--)| Indicates whether Refreshing Data or not. |
| [setRefreshDataFlag(boolean)](#setRefreshDataFlag-boolean-)| Indicates whether Refreshing Data or not. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--)| Gets the external connection data source. |
| [getDataSource()](#getDataSource--)| Gets and sets the data source of the pivot table. |
| [setDataSource(string[])](#setDataSource-stringarray-)| Gets and sets the data source of the pivot table. |
| [getPivotFormats()](#getPivotFormats--)| Gets the collection of formats applied to PivotTable. |
| [getItemPrintTitles()](#getItemPrintTitles--)| Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [setItemPrintTitles(boolean)](#setItemPrintTitles-boolean-)| Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [getPrintTitles()](#getPrintTitles--)| Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false. |
| [setPrintTitles(boolean)](#setPrintTitles-boolean-)| Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--)| Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true. |
| [setDisplayImmediateItems(boolean)](#setDisplayImmediateItems-boolean-)| Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true. |
| [isSelected()](#isSelected--)| Indicates whether this PivotTable is selected. |
| [setIsSelected(boolean)](#setIsSelected-boolean-)| Indicates whether this PivotTable is selected. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--)| Indicates whether the row header in the pivot table should have the style applied. |
| [setShowPivotStyleRowHeader(boolean)](#setShowPivotStyleRowHeader-boolean-)| Indicates whether the row header in the pivot table should have the style applied. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--)| Indicates whether the column header in the pivot table should have the style applied. |
| [setShowPivotStyleColumnHeader(boolean)](#setShowPivotStyleColumnHeader-boolean-)| Indicates whether the column header in the pivot table should have the style applied. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--)| Indicates whether row stripe formatting is applied. |
| [setShowPivotStyleRowStripes(boolean)](#setShowPivotStyleRowStripes-boolean-)| Indicates whether row stripe formatting is applied. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--)| Indicates whether stripe formatting is applied for column. |
| [setShowPivotStyleColumnStripes(boolean)](#setShowPivotStyleColumnStripes-boolean-)| Indicates whether stripe formatting is applied for column. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--)| Indicates whether the column formatting is applied. |
| [setShowPivotStyleLastColumn(boolean)](#setShowPivotStyleLastColumn-boolean-)| Indicates whether the column formatting is applied. |
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
| [changeDataSource(string[])](#changeDataSource-stringarray-)| Set pivottable's source data. Sheet1!$A$1:$C$3 |
| [getSource()](#getSource--)| Get pivottable's source data. |
| [refreshData()](#refreshData--)| Refreshes pivottable's data and setting from it's data source. |
| [refreshData(PivotTableRefreshOption)](#refreshData-pivottablerefreshoption-)| Refreshes pivottable's data and setting from it's data source with options. |
| [calculateData()](#calculateData--)| Calculates pivottable's data to cells. |
| [calculateData(PivotTableCalculateOption)](#calculateData-pivottablecalculateoption-)| Calculating pivot tables with options |
| [clearData()](#clearData--)| Clear PivotTable's data and formatting |
| [calculateRange()](#calculateRange--)| Calculates pivottable's range. |
| [formatAll(Style)](#formatAll-style-)| Format all the cell in the pivottable area |
| [formatRow(number, Style)](#formatRow-number-style-)| Format the row data in the pivottable area |
| [format(PivotArea, Style)](#format-pivotarea-style-)| Formats selected area of the PivotTable. |
| [format(number, number, Style)](#format-number-number-style-)| Format the cell in the pivottable area |
| [showInCompactForm()](#showInCompactForm--)| Layouts the PivotTable in compact form. |
| [showInOutlineForm()](#showInOutlineForm--)| Layouts the PivotTable in outline form. |
| [showInTabularForm()](#showInTabularForm--)| Layouts the PivotTable in tabular form. |
| [getCellByDisplayName(string)](#getCellByDisplayName-string-)| Gets the [Cell](../cell/) object by the display name of PivotField. |
| [getChildren()](#getChildren--)| Gets the Children Pivot Tables which use this PivotTable data as data source. |


### isExcel2003Compatible() {#isExcel2003Compatible--}

Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true.

```javascript
isExcel2003Compatible() : boolean;
```


### setIsExcel2003Compatible(boolean) {#setIsExcel2003Compatible-boolean-}

Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true.

```javascript
setIsExcel2003Compatible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshedByWho() {#getRefreshedByWho--}

Gets the name of the last user who refreshed this PivotTable

```javascript
getRefreshedByWho() : string;
```


### getRefreshDate() {#getRefreshDate--}

Gets the last date time when the PivotTable was refreshed.

```javascript
getRefreshDate() : Date;
```


### getPivotTableStyleName() {#getPivotTableStyleName--}

Gets and sets the pivottable style name.

```javascript
getPivotTableStyleName() : string;
```


### setPivotTableStyleName(string) {#setPivotTableStyleName-string-}

Gets and sets the pivottable style name.

```javascript
setPivotTableStyleName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPivotTableStyleType() {#getPivotTableStyleType--}

Gets and sets the built-in pivot table style.

```javascript
getPivotTableStyleType() : PivotTableStyleType;
```


**Returns**

[PivotTableStyleType](../pivottablestyletype/)

### setPivotTableStyleType(PivotTableStyleType) {#setPivotTableStyleType-pivottablestyletype-}

Gets and sets the built-in pivot table style.

```javascript
setPivotTableStyleType(value: PivotTableStyleType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotTableStyleType](../pivottablestyletype/) | The value to set. |

### getColumnFields() {#getColumnFields--}

Returns a PivotFields object that are currently shown as column fields.

```javascript
getColumnFields() : PivotFieldCollection;
```


**Returns**

[PivotFieldCollection](../pivotfieldcollection/)

### getRowFields() {#getRowFields--}

Returns a PivotFields object that are currently shown as row fields.

```javascript
getRowFields() : PivotFieldCollection;
```


**Returns**

[PivotFieldCollection](../pivotfieldcollection/)

### getPageFields() {#getPageFields--}

Returns a PivotFields object that are currently shown as page fields.

```javascript
getPageFields() : PivotFieldCollection;
```


**Returns**

[PivotFieldCollection](../pivotfieldcollection/)

### getDataFields() {#getDataFields--}

Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.

```javascript
getDataFields() : PivotFieldCollection;
```


**Returns**

[PivotFieldCollection](../pivotfieldcollection/)

### getDataField() {#getDataField--}

Gets a [PivotField](../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .

```javascript
getDataField() : PivotField;
```


**Returns**

[PivotField](../pivotfield/)

### getBaseFields() {#getBaseFields--}

Returns all base pivot fields in the PivotTable.

```javascript
getBaseFields() : PivotFieldCollection;
```


**Returns**

[PivotFieldCollection](../pivotfieldcollection/)

### getPivotFilters() {#getPivotFilters--}

Returns a list of pivot filters.

```javascript
getPivotFilters() : PivotFilterCollection;
```


**Returns**

[PivotFilterCollection](../pivotfiltercollection/)

### getColumnRange() {#getColumnRange--}

Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only.

```javascript
getColumnRange() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getRowRange() {#getRowRange--}

Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only.

```javascript
getRowRange() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getDataBodyRange() {#getDataBodyRange--}

Returns a [CellArea](../cellarea/) object that represents the range that contains the data area in the list between the header row and the insert row. Read-only.

```javascript
getDataBodyRange() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getTableRange1() {#getTableRange1--}

Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only.

```javascript
getTableRange1() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getTableRange2() {#getTableRange2--}

Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only.

```javascript
getTableRange2() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getColumnGrand() {#getColumnGrand--}

Indicates whether the PivotTable report shows grand totals for columns.

```javascript
getColumnGrand() : boolean;
```


### setColumnGrand(boolean) {#setColumnGrand-boolean-}

Indicates whether the PivotTable report shows grand totals for columns.

```javascript
setColumnGrand(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isGridDropZones() {#isGridDropZones--}

Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)

```javascript
isGridDropZones() : boolean;
```


### setIsGridDropZones(boolean) {#setIsGridDropZones-boolean-}

Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)

```javascript
setIsGridDropZones(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRowGrand() {#getRowGrand--}

Indicates whether the PivotTable report shows grand totals for rows.

```javascript
getRowGrand() : boolean;
```


### setRowGrand(boolean) {#setRowGrand-boolean-}

Indicates whether the PivotTable report shows grand totals for rows.

```javascript
setRowGrand(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDisplayNullString() {#getDisplayNullString--}

Indicates whether the PivotTable report displays a custom string if the value is null.

```javascript
getDisplayNullString() : boolean;
```


### setDisplayNullString(boolean) {#setDisplayNullString-boolean-}

Indicates whether the PivotTable report displays a custom string if the value is null.

```javascript
setDisplayNullString(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getNullString() {#getNullString--}

Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string.

```javascript
getNullString() : string;
```


### setNullString(string) {#setNullString-string-}

Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string.

```javascript
setNullString(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDisplayErrorString() {#getDisplayErrorString--}

Indicates whether the PivotTable report displays a custom string in cells that contain errors.

```javascript
getDisplayErrorString() : boolean;
```


### setDisplayErrorString(boolean) {#setDisplayErrorString-boolean-}

Indicates whether the PivotTable report displays a custom string in cells that contain errors.

```javascript
setDisplayErrorString(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDataFieldHeaderName() {#getDataFieldHeaderName--}

Gets and sets the name of the value area field header in the PivotTable.

```javascript
getDataFieldHeaderName() : string;
```


### setDataFieldHeaderName(string) {#setDataFieldHeaderName-string-}

Gets and sets the name of the value area field header in the PivotTable.

```javascript
setDataFieldHeaderName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getErrorString() {#getErrorString--}

Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string.

```javascript
getErrorString() : string;
```


### setErrorString(string) {#setErrorString-string-}

Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string.

```javascript
setErrorString(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isAutoFormat() {#isAutoFormat--}

Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003

```javascript
isAutoFormat() : boolean;
```


### setIsAutoFormat(boolean) {#setIsAutoFormat-boolean-}

Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003

```javascript
setIsAutoFormat(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}

Indicates whether autofitting column width on update

```javascript
getAutofitColumnWidthOnUpdate() : boolean;
```


### setAutofitColumnWidthOnUpdate(boolean) {#setAutofitColumnWidthOnUpdate-boolean-}

Indicates whether autofitting column width on update

```javascript
setAutofitColumnWidthOnUpdate(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAutoFormatType() {#getAutoFormatType--}

Gets and sets the auto format type of PivotTable.

```javascript
getAutoFormatType() : PivotTableAutoFormatType;
```


**Returns**

[PivotTableAutoFormatType](../pivottableautoformattype/)

### setAutoFormatType(PivotTableAutoFormatType) {#setAutoFormatType-pivottableautoformattype-}

Gets and sets the auto format type of PivotTable.

```javascript
setAutoFormatType(value: PivotTableAutoFormatType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotTableAutoFormatType](../pivottableautoformattype/) | The value to set. |

### getHasBlankRows() {#getHasBlankRows--}

Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.

```javascript
getHasBlankRows() : boolean;
```


### setHasBlankRows(boolean) {#setHasBlankRows-boolean-}

Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.

```javascript
setHasBlankRows(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMergeLabels() {#getMergeLabels--}

True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells.

```javascript
getMergeLabels() : boolean;
```


### setMergeLabels(boolean) {#setMergeLabels-boolean-}

True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells.

```javascript
setMergeLabels(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPreserveFormatting() {#getPreserveFormatting--}

Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated.

```javascript
getPreserveFormatting() : boolean;
```


### setPreserveFormatting(boolean) {#setPreserveFormatting-boolean-}

Indicates whether formatting is preserved when the PivotTable is refreshed or recalculated.

```javascript
setPreserveFormatting(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowDrill() {#getShowDrill--}

Gets and sets whether showing expand/collapse buttons.

```javascript
getShowDrill() : boolean;
```


### setShowDrill(boolean) {#setShowDrill-boolean-}

Gets and sets whether showing expand/collapse buttons.

```javascript
setShowDrill(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEnableDrilldown() {#getEnableDrilldown--}

Gets whether drilldown is enabled.

```javascript
getEnableDrilldown() : boolean;
```


### setEnableDrilldown(boolean) {#setEnableDrilldown-boolean-}

Gets whether drilldown is enabled.

```javascript
setEnableDrilldown(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEnableFieldDialog() {#getEnableFieldDialog--}

Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field.

```javascript
getEnableFieldDialog() : boolean;
```


### setEnableFieldDialog(boolean) {#setEnableFieldDialog-boolean-}

Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field.

```javascript
setEnableFieldDialog(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEnableFieldList() {#getEnableFieldList--}

Gets whether enable the field list for the PivotTable.

```javascript
getEnableFieldList() : boolean;
```


### setEnableFieldList(boolean) {#setEnableFieldList-boolean-}

Gets whether enable the field list for the PivotTable.

```javascript
setEnableFieldList(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEnableWizard() {#getEnableWizard--}

Indicates whether the PivotTable Wizard is available.

```javascript
getEnableWizard() : boolean;
```


### setEnableWizard(boolean) {#setEnableWizard-boolean-}

Indicates whether the PivotTable Wizard is available.

```javascript
setEnableWizard(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}

Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False.

```javascript
getSubtotalHiddenPageItems() : boolean;
```


### setSubtotalHiddenPageItems(boolean) {#setSubtotalHiddenPageItems-boolean-}

Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False.

```javascript
setSubtotalHiddenPageItems(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getGrandTotalName() {#getGrandTotalName--}

Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total".

```javascript
getGrandTotalName() : string;
```


### setGrandTotalName(string) {#setGrandTotalName-string-}

Returns the text string label that is displayed in the grand total column or row heading. The default value is the string "Grand Total".

```javascript
setGrandTotalName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getManualUpdate() {#getManualUpdate--}

Indicates whether the PivotTable report is recalculated only at the user's request.

```javascript
getManualUpdate() : boolean;
```


### setManualUpdate(boolean) {#setManualUpdate-boolean-}

Indicates whether the PivotTable report is recalculated only at the user's request.

```javascript
setManualUpdate(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isMultipleFieldFilters() {#isMultipleFieldFilters--}

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

```javascript
isMultipleFieldFilters() : boolean;
```


### setIsMultipleFieldFilters(boolean) {#setIsMultipleFieldFilters-boolean-}

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

```javascript
setIsMultipleFieldFilters(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMissingItemsLimit() {#getMissingItemsLimit--}

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

```javascript
getMissingItemsLimit() : PivotMissingItemLimitType;
```


**Returns**

[PivotMissingItemLimitType](../pivotmissingitemlimittype/)

### setMissingItemsLimit(PivotMissingItemLimitType) {#setMissingItemsLimit-pivotmissingitemlimittype-}

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

```javascript
setMissingItemsLimit(value: PivotMissingItemLimitType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotMissingItemLimitType](../pivotmissingitemlimittype/) | The value to set. |

### getEnableDataValueEditing() {#getEnableDataValueEditing--}

Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area

```javascript
getEnableDataValueEditing() : boolean;
```


### setEnableDataValueEditing(boolean) {#setEnableDataValueEditing-boolean-}

Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area

```javascript
setEnableDataValueEditing(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowDataTips() {#getShowDataTips--}

Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells.

```javascript
getShowDataTips() : boolean;
```


### setShowDataTips(boolean) {#setShowDataTips-boolean-}

Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells.

```javascript
setShowDataTips(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}

Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips.

```javascript
getShowMemberPropertyTips() : boolean;
```


### setShowMemberPropertyTips(boolean) {#setShowMemberPropertyTips-boolean-}

Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips.

```javascript
setShowMemberPropertyTips(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowValuesRow() {#getShowValuesRow--}

Specifies a boolean value that indicates whether show values row. show the values row

```javascript
getShowValuesRow() : boolean;
```


### setShowValuesRow(boolean) {#setShowValuesRow-boolean-}

Specifies a boolean value that indicates whether show values row. show the values row

```javascript
setShowValuesRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowEmptyCol() {#getShowEmptyCol--}

Specifies a boolean value that indicates whether to include empty columns in the table

```javascript
getShowEmptyCol() : boolean;
```


### setShowEmptyCol(boolean) {#setShowEmptyCol-boolean-}

Specifies a boolean value that indicates whether to include empty columns in the table

```javascript
setShowEmptyCol(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowEmptyRow() {#getShowEmptyRow--}

Specifies a boolean value that indicates whether to include empty rows in the table.

```javascript
getShowEmptyRow() : boolean;
```


### setShowEmptyRow(boolean) {#setShowEmptyRow-boolean-}

Specifies a boolean value that indicates whether to include empty rows in the table.

```javascript
setShowEmptyRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFieldListSortAscending() {#getFieldListSortAscending--}

Indicates whether fields in the PivotTable are sorted in non-default order in the field list.

```javascript
getFieldListSortAscending() : boolean;
```


### setFieldListSortAscending(boolean) {#setFieldListSortAscending-boolean-}

Indicates whether fields in the PivotTable are sorted in non-default order in the field list.

```javascript
setFieldListSortAscending(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPrintDrill() {#getPrintDrill--}

Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable.

```javascript
getPrintDrill() : boolean;
```


### setPrintDrill(boolean) {#setPrintDrill-boolean-}

Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable.

```javascript
setPrintDrill(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAltTextTitle() {#getAltTextTitle--}

Gets the title of the altertext

```javascript
getAltTextTitle() : string;
```


### setAltTextTitle(string) {#setAltTextTitle-string-}

Gets the title of the altertext

```javascript
setAltTextTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAltTextDescription() {#getAltTextDescription--}

Gets the description of the alt text

```javascript
getAltTextDescription() : string;
```


### setAltTextDescription(string) {#setAltTextDescription-string-}

Gets the description of the alt text

```javascript
setAltTextDescription(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getName() {#getName--}

Gets the name of the PivotTable

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets the name of the PivotTable

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getColumnHeaderCaption() {#getColumnHeaderCaption--}

Gets the Column Header Caption of the PivotTable.

```javascript
getColumnHeaderCaption() : string;
```


### setColumnHeaderCaption(string) {#setColumnHeaderCaption-string-}

Gets the Column Header Caption of the PivotTable.

```javascript
setColumnHeaderCaption(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getIndent() {#getIndent--}

Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.

```javascript
getIndent() : number;
```


### setIndent(number) {#setIndent-number-}

Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.

```javascript
setIndent(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getRowHeaderCaption() {#getRowHeaderCaption--}

Gets the Row Header Caption of the PivotTable.

```javascript
getRowHeaderCaption() : string;
```


### setRowHeaderCaption(string) {#setRowHeaderCaption-string-}

Gets the Row Header Caption of the PivotTable.

```javascript
setRowHeaderCaption(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}

Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs

```javascript
getShowRowHeaderCaption() : boolean;
```


### setShowRowHeaderCaption(boolean) {#setShowRowHeaderCaption-boolean-}

Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs

```javascript
setShowRowHeaderCaption(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCustomListSort() {#getCustomListSort--}

Indicates whether consider built-in custom list when sort data

```javascript
getCustomListSort() : boolean;
```


### setCustomListSort(boolean) {#setCustomListSort-boolean-}

Indicates whether consider built-in custom list when sort data

```javascript
setCustomListSort(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPivotFormatConditions() {#getPivotFormatConditions--}

Gets the Format Conditions of the pivot table.

```javascript
getPivotFormatConditions() : PivotFormatConditionCollection;
```


**Returns**

[PivotFormatConditionCollection](../pivotformatconditioncollection/)

### getPageFieldOrder() {#getPageFieldOrder--}

Gets the order in which page fields are added to the PivotTable report's layout.

```javascript
getPageFieldOrder() : PrintOrderType;
```


**Returns**

[PrintOrderType](../printordertype/)

### setPageFieldOrder(PrintOrderType) {#setPageFieldOrder-printordertype-}

Gets the order in which page fields are added to the PivotTable report's layout.

```javascript
setPageFieldOrder(value: PrintOrderType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintOrderType](../printordertype/) | The value to set. |

### getPageFieldWrapCount() {#getPageFieldWrapCount--}

Gets the number of page fields in each column or row in the PivotTable report.

```javascript
getPageFieldWrapCount() : number;
```


### setPageFieldWrapCount(number) {#setPageFieldWrapCount-number-}

Gets the number of page fields in each column or row in the PivotTable report.

```javascript
setPageFieldWrapCount(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTag() {#getTag--}

Gets a string saved with the PivotTable report.

```javascript
getTag() : string;
```


### setTag(string) {#setTag-string-}

Gets a string saved with the PivotTable report.

```javascript
setTag(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSaveData() {#getSaveData--}

Indicates whether data for the PivotTable report is saved with the workbook.

```javascript
getSaveData() : boolean;
```


### setSaveData(boolean) {#setSaveData-boolean-}

Indicates whether data for the PivotTable report is saved with the workbook.

```javascript
setSaveData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}

Indicates whether Refresh Data when Opening File.

```javascript
getRefreshDataOnOpeningFile() : boolean;
```


### setRefreshDataOnOpeningFile(boolean) {#setRefreshDataOnOpeningFile-boolean-}

Indicates whether Refresh Data when Opening File.

```javascript
setRefreshDataOnOpeningFile(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshDataFlag() {#getRefreshDataFlag--}

Indicates whether Refreshing Data or not.

```javascript
getRefreshDataFlag() : boolean;
```


### setRefreshDataFlag(boolean) {#setRefreshDataFlag-boolean-}

Indicates whether Refreshing Data or not.

```javascript
setRefreshDataFlag(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}

Gets the external connection data source.

```javascript
getExternalConnectionDataSource() : ExternalConnection;
```


**Returns**

[ExternalConnection](../externalconnection/)

### getDataSource() {#getDataSource--}

Gets and sets the data source of the pivot table.

```javascript
getDataSource() : string[];
```


**Returns**

string[]

### setDataSource(string[]) {#setDataSource-stringarray-}

Gets and sets the data source of the pivot table.

```javascript
setDataSource(value: string[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string[] | The value to set. |

### getPivotFormats() {#getPivotFormats--}

Gets the collection of formats applied to PivotTable.

```javascript
getPivotFormats() : PivotTableFormatCollection;
```


**Returns**

[PivotTableFormatCollection](../pivottableformatcollection/)

### getItemPrintTitles() {#getItemPrintTitles--}

Indicates whether PivotItem names should be repeated at the top of each printed page.

```javascript
getItemPrintTitles() : boolean;
```


### setItemPrintTitles(boolean) {#setItemPrintTitles-boolean-}

Indicates whether PivotItem names should be repeated at the top of each printed page.

```javascript
setItemPrintTitles(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPrintTitles() {#getPrintTitles--}

Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false.

```javascript
getPrintTitles() : boolean;
```


### setPrintTitles(boolean) {#setPrintTitles-boolean-}

Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false.

```javascript
setPrintTitles(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDisplayImmediateItems() {#getDisplayImmediateItems--}

Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true.

```javascript
getDisplayImmediateItems() : boolean;
```


### setDisplayImmediateItems(boolean) {#setDisplayImmediateItems-boolean-}

Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true.

```javascript
setDisplayImmediateItems(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isSelected() {#isSelected--}

Indicates whether this PivotTable is selected.

```javascript
isSelected() : boolean;
```


### setIsSelected(boolean) {#setIsSelected-boolean-}

Indicates whether this PivotTable is selected.

```javascript
setIsSelected(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}

Indicates whether the row header in the pivot table should have the style applied.

```javascript
getShowPivotStyleRowHeader() : boolean;
```


### setShowPivotStyleRowHeader(boolean) {#setShowPivotStyleRowHeader-boolean-}

Indicates whether the row header in the pivot table should have the style applied.

```javascript
setShowPivotStyleRowHeader(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}

Indicates whether the column header in the pivot table should have the style applied.

```javascript
getShowPivotStyleColumnHeader() : boolean;
```


### setShowPivotStyleColumnHeader(boolean) {#setShowPivotStyleColumnHeader-boolean-}

Indicates whether the column header in the pivot table should have the style applied.

```javascript
setShowPivotStyleColumnHeader(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}

Indicates whether row stripe formatting is applied.

```javascript
getShowPivotStyleRowStripes() : boolean;
```


### setShowPivotStyleRowStripes(boolean) {#setShowPivotStyleRowStripes-boolean-}

Indicates whether row stripe formatting is applied.

```javascript
setShowPivotStyleRowStripes(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}

Indicates whether stripe formatting is applied for column.

```javascript
getShowPivotStyleColumnStripes() : boolean;
```


### setShowPivotStyleColumnStripes(boolean) {#setShowPivotStyleColumnStripes-boolean-}

Indicates whether stripe formatting is applied for column.

```javascript
setShowPivotStyleColumnStripes(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}

Indicates whether the column formatting is applied.

```javascript
getShowPivotStyleLastColumn() : boolean;
```


### setShowPivotStyleLastColumn(boolean) {#setShowPivotStyleLastColumn-boolean-}

Indicates whether the column formatting is applied.

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

### move(string) {#move-string-}

Moves the PivotTable to a different location in the worksheet.

```javascript
move(destCellName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destCellName | string | the dest cell name. |

### changeDataSource(string[]) {#changeDataSource-stringarray-}

Set pivottable's source data. Sheet1!$A$1:$C$3

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

### refreshData() {#refreshData--}

Refreshes pivottable's data and setting from it's data source.

```javascript
refreshData() : void;
```


**Remarks**

We will gather data from data source to a pivot cache ,then calculate the data in the cache to the cells. This method is only used to gather all data to a pivot cache.

### refreshData(PivotTableRefreshOption) {#refreshData-pivottablerefreshoption-}

Refreshes pivottable's data and setting from it's data source with options.

```javascript
refreshData(option: PivotTableRefreshOption) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../pivottablerefreshoption/) | The options for refreshing data source of pivot table. |

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
| pivotArea | [PivotArea](../pivotarea/) |  |
| style | [Style](../style/) |  |

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


