---
title: "ListObject Class"
linktitle: "ListObject"
articleTitle: "ListObject"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a list object on a worksheet."
type: docs
weight: 3440
url: /python-java/asposecells.api/listobject/
---

## ListObject class

Represents a list object on a worksheet. The ListObject object is a member of the ListObjects collection. The ListObjects collection contains all the list objects on a worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [StartRow](#startrow) | int | Gets the start row of the range. |
| [StartColumn](#startcolumn) | int | Gets the start column of the range. |
| [EndRow](#endrow) | int | Gets the end row of the range. |
| [EndColumn](#endcolumn) | int | Gets the end column of the range. |
| [ListColumns](#listcolumns) | ListColumnCollection | Gets ListColumns of the ListObject. |
| [ShowHeaderRow](#showheaderrow) | boolean | Gets and sets whether this ListObject show header row. |
| [ShowTotals](#showtotals) | boolean | Gets and sets whether this ListObject show total row. |
| [DataRange](#datarange) | Range | Gets the data range of the ListObject. |
| [QueryTable](#querytable) | QueryTable | Gets the linked QueryTable. |
| [DataSourceType](#datasourcetype) | int | Gets the data source type of the table. The value of the property is TableDataSourceType integer constant. |
| [HasAutoFilter](#hasautofilter) | boolean |  |
| [AutoFilter](#autofilter) | AutoFilter | Gets auto filter. |
| [DisplayName](#displayname) | String | Gets and sets the display name. |
| [Comment](#comment) | String | Gets and sets the comment of the table. |
| [ShowTableStyleFirstColumn](#showtablestylefirstcolumn) | boolean | Indicates whether the first column in the table should have the style applied. |
| [ShowTableStyleLastColumn](#showtablestylelastcolumn) | boolean | Indicates whether the last column in the table should have the style applied. |
| [ShowTableStyleRowStripes](#showtablestylerowstripes) | boolean | Indicates whether row stripe formatting is applied. |
| [ShowTableStyleColumnStripes](#showtablestylecolumnstripes) | boolean | Indicates whether column stripe formatting is applied. |
| [TableStyleType](#tablestyletype) | int | Gets and the built-in table style. The value of the property is TableStyleType integer constant. |
| [TableStyleName](#tablestylename) | String | Gets and sets the table style name. |
| [XmlMap](#xmlmap) | XmlMap | Gets an XmlMap used for this list. |
| [AlternativeText](#alternativetext) | String | Gets and sets the alternative text. |
| [AlternativeDescription](#alternativedescription) | String | Gets and sets the alternative description. |

## Methods

| Name | Description |
| --- | --- |
| [resize](#resize) | Resize the range of the list object. |
| [putCellValue](#putcellvalue) | Put the value to the cell. |
| [putCellFormula](#putcellformula) | Put the formula to the cell in the table. |
| [updateColumnName](#updatecolumnname) | Updates all list columns' name from the worksheet.

The value of the cells in the header row of the table must be same a |
| [removeAutoFilter](#removeautofilter) |  |
| [filter](#filter) | Filter the table. |
| [applyStyleToRange](#applystyletorange) | Apply the table style to the range. |
| [convertToRange](#converttorange) | Convert the table to range. |

### ListObject.StartRow property {#startrow}

Gets the start row of the range.

**Type:** int

### ListObject.StartColumn property {#startcolumn}

Gets the start column of the range.

**Type:** int

### ListObject.EndRow property {#endrow}

Gets the end row of the range.

**Type:** int

### ListObject.EndColumn property {#endcolumn}

Gets the end column of the range.

**Type:** int

### ListObject.ListColumns property {#listcolumns}

Gets ListColumns of the ListObject.

**Type:** ListColumnCollection

### ListObject.ShowHeaderRow property {#showheaderrow}

Gets and sets whether this ListObject show header row.

**Type:** boolean

### ListObject.ShowTotals property {#showtotals}

Gets and sets whether this ListObject show total row.

**Type:** boolean

### ListObject.DataRange property {#datarange}

Gets the data range of the ListObject.

**Type:** Range

### ListObject.QueryTable property {#querytable}

Gets the linked QueryTable.

**Type:** QueryTable

### ListObject.DataSourceType property {#datasourcetype}

Gets the data source type of the table. The value of the property is TableDataSourceType integer constant.

**Type:** int

### ListObject.HasAutoFilter property {#hasautofilter}

**Type:** boolean

### ListObject.AutoFilter property {#autofilter}

Gets auto filter.

**Type:** AutoFilter

### ListObject.DisplayName property {#displayname}

Gets and sets the display name.

**Type:** String

### ListObject.Comment property {#comment}

Gets and sets the comment of the table.

**Type:** String

### ListObject.ShowTableStyleFirstColumn property {#showtablestylefirstcolumn}

Indicates whether the first column in the table should have the style applied.

**Type:** boolean

### ListObject.ShowTableStyleLastColumn property {#showtablestylelastcolumn}

Indicates whether the last column in the table should have the style applied.

**Type:** boolean

### ListObject.ShowTableStyleRowStripes property {#showtablestylerowstripes}

Indicates whether row stripe formatting is applied.

**Type:** boolean

### ListObject.ShowTableStyleColumnStripes property {#showtablestylecolumnstripes}

Indicates whether column stripe formatting is applied.

**Type:** boolean

### ListObject.TableStyleType property {#tablestyletype}

Gets and the built-in table style. The value of the property is TableStyleType integer constant.

**Type:** int

### ListObject.TableStyleName property {#tablestylename}

Gets and sets the table style name.

**Type:** String

### ListObject.XmlMap property {#xmlmap}

Gets an XmlMap used for this list.

**Type:** XmlMap

### ListObject.AlternativeText property {#alternativetext}

Gets and sets the alternative text.

**Type:** String

### ListObject.AlternativeDescription property {#alternativedescription}

Gets and sets the alternative description.

**Type:** String

### resize(startRow, startColumn, endRow, endColumn, hasHeaders) {#resize}

Resize the range of the list object.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row index of the new range. |
| startColumn | int | The start column index of the new range. |
| endRow | int | The end row index of the new range. |
| endColumn | int | The end column index of the new range. |
| hasHeaders | boolean | Whether this table has headers. |

### putCellValue(rowOffset, columnOffset, value) (1 of 2) {#putcellvalue}

Put the value to the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | The row offset in the table. |
| columnOffset | int | The column offset in the table. |
| value | Object | The cell value. |

---

### putCellValue(rowOffset, columnOffset, value, isTotalsRowLabel) (2 of 2) {#putcellvalue-1}

Put the value to the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | The row offset in the table. |
| columnOffset | int | The column offset in the table. |
| value | Object | The cell value. |
| isTotalsRowLabel | boolean | Indicates whether it is a label for total row,only works for total row. If False and this row is total row, a new row will be inserted. |

### putCellFormula(rowOffset, columnOffset, formula) (1 of 2) {#putcellformula}

Put the formula to the cell in the table.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | The row offset in the table. |
| columnOffset | int | The column offset in the table. |
| formula | String | The formula of the cell. |

---

### putCellFormula(rowOffset, columnOffset, formula, isTotalsRowFormula) (2 of 2) {#putcellformula-1}

Put the formula to the cell in the table.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int | The row offset in the table. |
| columnOffset | int | The column offset in the table. |
| formula | String | The formula of the cell. |
| isTotalsRowFormula | boolean |  |

### updateColumnName() {#updatecolumnname}

Updates all list columns' name from the worksheet.

The value of the cells in the header row of the table must be same as the name of the ListColumn; Cell.PutValue do not auto modify the name of the ListColumn for performance.

### removeAutoFilter() {#removeautofilter}

### filter() {#filter}

Filter the table.

### applyStyleToRange() {#applystyletorange}

Apply the table style to the range.

### convertToRange() (1 of 2) {#converttorange}

Convert the table to range.

---

### convertToRange(options) (2 of 2) {#converttorange-1}

Convert the table to range.

| Parameter | Type | Description |
| --- | --- | --- |
| options | TableToRangeOptions | the options when converting table to range. |
