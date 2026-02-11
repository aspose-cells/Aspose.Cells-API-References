---
title: PivotTable
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Summary description for PivotTable.
type: docs
url: /javascript-cpp/pivottable/
---

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
| [pivotTableStyle](#pivotTableStyle--)| TableStyle | Gets [TableStyle](../tablestyle/) settings of this pivot table. |
| [pivotTableStyleName](#pivotTableStyleName--)| string | Gets and sets the pivottable style name. |
| [pivotTableStyleType](#pivotTableStyleType--)| PivotTableStyleType | Gets and sets the built-in pivot table style. |
| [columnFields](#columnFields--)| PivotFieldCollection | Readonly. Returns a PivotFields object that are currently shown as column fields. |
| [rowFields](#rowFields--)| PivotFieldCollection | Readonly. Returns a PivotFields object that are currently shown as row fields. |
| [pageFields](#pageFields--)| PivotFieldCollection | Readonly. Returns a PivotFields object that are currently shown as page fields. |
| [dataFields](#dataFields--)| PivotFieldCollection | Readonly. Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area. |
| [dataField](#dataField--)| PivotField | Readonly. Gets a [PivotField](../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method . |
| [valuesField](#valuesField--)| PivotField | Readonly. Gets a [PivotField](../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method . |
| [baseFields](#baseFields--)| PivotFieldCollection | Readonly. Returns all base pivot fields in the PivotTable. |
| [pivotFilters](#pivotFilters--)| PivotFilterCollection | Readonly. Returns all filters of pivot fields in the pivot table. |
| [topRightArea](#topRightArea--)| CellArea | Readonly. Represents the blank area at the top-right of the PivotTable (top-left for RTL sheets). |
| [filterArea](#filterArea--)| CellArea | Readonly. Gets the region of filter region. |
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
| [printDrill](#printDrill--)| boolean | Specifies a boolean value that indicates whether drill indicators should be printed. Print expand/collapse buttons when displayed on pivottable. |
| [altTextTitle](#altTextTitle--)| string | Gets and sets the title of the alter text. |
| [altTextDescription](#altTextDescription--)| string | Gets the description of the alt text. |
| [name](#name--)| string | Gets the name of the PivotTable |
| [columnHeaderCaption](#columnHeaderCaption--)| string | Gets and sets the custom Caption of the Column Header of the PivotTable. |
| [indent](#indent--)| number | Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form. |
| [rowHeaderCaption](#rowHeaderCaption--)| string | Gets and sets custom caption of the Row Header in this PivotTable. |
| [showRowHeaderCaption](#showRowHeaderCaption--)| boolean | Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs |
| [customListSort](#customListSort--)| boolean | Indicates whether consider built-in custom list when sort data |
| [pivotFormatConditions](#pivotFormatConditions--)| PivotFormatConditionCollection | Readonly. Gets the Format Conditions of the pivot table. |
| [conditionalFormats](#conditionalFormats--)| PivotConditionalFormatCollection | Readonly. Gets the conditional formats of the pivot table. |
| [pageFieldOrder](#pageFieldOrder--)| PrintOrderType | Gets and sets the order in which page fields are added to the PivotTable report's layout. |
| [pageFieldWrapCount](#pageFieldWrapCount--)| number | Gets the number of page fields in each column or row in the PivotTable report. |
| [tag](#tag--)| string | Gets and sets a user-defined string that is associated with this PivotTable view. |
| [saveData](#saveData--)| boolean | Indicates whether data for the PivotTable report is saved with the workbook. |
| [refreshDataOnOpeningFile](#refreshDataOnOpeningFile--)| boolean | Indicates whether Refresh Data when Opening File. |
| [refreshDataFlag](#refreshDataFlag--)| boolean | Indicates whether Refreshing Data or not. |
| [sourceType](#sourceType--)| PivotTableSourceType | Readonly. Gets the data source type of the pivot table. |
| [externalConnectionDataSource](#externalConnectionDataSource--)| ExternalConnection | Readonly. Gets the external connection data source. |
| [dataSource](#dataSource--)| string[] | Gets and sets the data source of the pivot table. |
| [pivotFormats](#pivotFormats--)| PivotTableFormatCollection | Readonly. Gets all formats applied to PivotTable. |
| [itemPrintTitles](#itemPrintTitles--)| boolean | Indicates whether PivotItem names should be repeated at the top of each printed page. |
| [repeatItemsOnEachPrintedPage](#repeatItemsOnEachPrintedPage--)| boolean | Indicates whether captions of pivot item  on the row area are repeated on each printed page for pivot fields in tabular form. |
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
| [getButtonArea(PivotFieldType)](#getButtonArea-pivotfieldtype-)| Gets the area contains field button. |
| [move(number, number)](#move-number-number-)| Moves the PivotTable to a different location in the worksheet. |
| [move(string)](#move-string-)| Moves the PivotTable to a different location in the worksheet. |
| [moveTo(number, number)](#moveTo-number-number-)| Moves the PivotTable to a different location in the worksheet. |
| [moveTo(string)](#moveTo-string-)| Moves the PivotTable to a different location in the worksheet. |
| [getSourceDataConnections()](#getSourceDataConnections--)| Gets the external connection data sources. |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--)| Gets the names of external source data connections. |
| [changeDataSource(string[])](#changeDataSource-stringarray-)| Change data source of the pivottable. |
| [getSource()](#getSource--)| Get the data source of this pivottable. |
| [getSource(boolean)](#getSource-boolean-)| Get the data source of this pivottable. |
| [refreshData()](#refreshData--)| Refreshes pivottable's data and setting from it's data source. |
| [refreshData(PivotTableRefreshOption)](#refreshData-pivottablerefreshoption-)| Refreshes pivottable's data and setting from it's data source with options. |
| [calculateData()](#calculateData--)| Calculates data of pivottable to cells. |
| [calculateData(PivotTableCalculateOption)](#calculateData-pivottablecalculateoption-)| Calculates pivot table with options. |
| [clearData()](#clearData--)| Clear data and formatting of PivotTable view. |
| [calculateRange()](#calculateRange--)| Calculates pivottable's range. |
| [formatAll(Style)](#formatAll-style-)| Format all the cell in the pivottable area |
| [formatRow(number, Style)](#formatRow-number-style-)| Format the row data in the pivottable area |
| [format(PivotArea, Style)](#format-pivotarea-style-)| Formats selected area of the PivotTable. |
| [format(CellArea, Style)](#format-cellarea-style-)| Formats selected area of the PivotTable. |
| [format(number, number, Style)](#format-number-number-style-)| Formats the cell in the pivottable area |
| [selectArea(CellArea)](#selectArea-cellarea-)| Select an area of pivot table view. |
| [showDetail(number, number, boolean, number, number)](#showDetail-number-number-boolean-number-number-)| Show the detail of one item in the data region to a new Table. |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--)| Gets horizontal page breaks of this pivot table. |
| [showInCompactForm()](#showInCompactForm--)| Layouts the PivotTable view in compact form. |
| [showInOutlineForm()](#showInOutlineForm--)| Layouts the PivotTable in outline form. |
| [showInTabularForm()](#showInTabularForm--)| Layouts the PivotTable in tabular form. |
| [getCellByDisplayName(string)](#getCellByDisplayName-string-)| Gets the [Cell](../cell/) object by the display name of PivotField. |
| [getChildren()](#getChildren--)| Gets the Children Pivot Tables which use this PivotTable data as data source. |


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


### pivotTableStyle {#pivotTableStyle--}

Gets [TableStyle](../tablestyle/) settings of this pivot table.

```javascript
pivotTableStyle : TableStyle;
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


**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotTable.ValuesField property. This method will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### valuesField {#valuesField--}

Readonly. Gets a [PivotField](../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .

```javascript
valuesField : PivotField;
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


### topRightArea {#topRightArea--}

Readonly. Represents the blank area at the top-right of the PivotTable (top-left for RTL sheets).

```javascript
topRightArea : CellArea;
```


### filterArea {#filterArea--}

Readonly. Gets the region of filter region.

```javascript
filterArea : CellArea;
```


**Remarks**

Only valid if filter pivot fields exists.

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

Specifies a boolean value that indicates whether drill indicators should be printed. Print expand/collapse buttons when displayed on pivottable.

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

Gets and sets the custom Caption of the Column Header of the PivotTable.

```javascript
columnHeaderCaption : string;
```


### indent {#indent--}

Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.

```javascript
indent : number;
```


### rowHeaderCaption {#rowHeaderCaption--}

Gets and sets custom caption of the Row Header in this PivotTable.

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

Gets and sets a user-defined string that is associated with this PivotTable view.

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

Readonly. Gets all formats applied to PivotTable.

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

Indicates whether captions of pivot item  on the row area are repeated on each printed page for pivot fields in tabular form.

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

### getButtonArea(PivotFieldType) {#getButtonArea-pivotfieldtype-}

Gets the area contains field button.

```javascript
getButtonArea(axisType: PivotFieldType) : CellArea;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region type. |

**Returns**

[CellArea](../cellarea/)

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

Gets the names of external source data connections.

```javascript
getNamesOfSourceDataConnections() : string[];
```


**Returns**

string[]

### changeDataSource(string[]) {#changeDataSource-stringarray-}

Change data source of the pivottable.

```javascript
changeDataSource(source: string[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | string[] |  |

### getSource() {#getSource--}

Get the data source of this pivottable.

```javascript
getSource() : string[];
```


**Returns**

string[]

### getSource(boolean) {#getSource-boolean-}

Get the data source of this pivottable.

```javascript
getSource(isOriginal: boolean) : string[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isOriginal | boolean | Indicates whether to return original or display data source. |

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

Calculates data of pivottable to cells.

```javascript
calculateData() : void;
```


**Remarks**

Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.

### calculateData(PivotTableCalculateOption) {#calculateData-pivottablecalculateoption-}

Calculates pivot table with options.

```javascript
calculateData(option: PivotTableCalculateOption) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../pivottablecalculateoption/) | The options for calculating the pivot table |

**Remarks**

If PivotTableCalculateOption.RefreshData is true, this method will refresh pivot cache from data source,then calculate all pivot tables based same pivot cache.

### clearData() {#clearData--}

Clear data and formatting of PivotTable view.

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

Formats the cell in the pivottable area

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

Layouts the PivotTable view in compact form.

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


