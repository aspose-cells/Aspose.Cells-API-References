---
title: ListObject
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a table in a worksheet.
type: docs
url: /javascript-cpp/listobject/
---

## ListObject class

Represents a table in a worksheet.

```javascript
class ListObject;
```


### Example
```javascript
const { Workbook, CellsHelper, TotalsCalculation, SaveFormat } = AsposeCells;

var workbook = new Workbook();
var cells = workbook.worksheets.get(0).cells;
for (var i = 0; i < 5; i++) {
    cells.get(0, i).putValue(CellsHelper.columnIndexToName(i));
}
for (var row = 1; row < 10; row++) {
    for (var column = 0; column < 5; column++) {
        cells.get(row, column).putValue(row * column);
    }
}
var tables = workbook.worksheets.get(0).getListObjects();
var index = tables.add(0, 0, 9, 4, true);
var table = tables.get(0);
table.showTotals = true;
table.listColumns.get(4).totalsCalculation = TotalsCalculation.Sum;
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [startRow](#startRow--)| number | Readonly. Gets the start row of the range. |
| [startColumn](#startColumn--)| number | Readonly. Gets the start column of the range. |
| [endRow](#endRow--)| number | Readonly. Gets the end  row of the range. |
| [endColumn](#endColumn--)| number | Readonly. Gets the end column of the range. |
| [listColumns](#listColumns--)| ListColumnCollection | Readonly. Gets the [ListColumn](../listcolumn/) list of this table. |
| [showHeaderRow](#showHeaderRow--)| boolean | Gets and sets whether this Table shows header row. |
| [showTotals](#showTotals--)| boolean | Gets and sets whether this TAble shows total row. |
| [dataRange](#dataRange--)| Range | Readonly. Gets the data range of the Table. |
| [queryTable](#queryTable--)| QueryTable | Readonly. Gets the linked QueryTable. |
| [dataSourceType](#dataSourceType--)| TableDataSourceType | Readonly. Gets the data source type of the table. |
| [hasAutoFilter](#hasAutoFilter--)| boolean | Indicates whether auto filter is applied to this table. |
| [autoFilter](#autoFilter--)| AutoFilter | Readonly. Gets auto filter of this table. |
| [displayName](#displayName--)| string | Gets and sets the display name of the table. |
| [comment](#comment--)| string | Gets and sets the comment of the table. |
| [showTableStyleFirstColumn](#showTableStyleFirstColumn--)| boolean | Indicates whether the first column in the table is the style applied to. |
| [showTableStyleLastColumn](#showTableStyleLastColumn--)| boolean | Indicates whether the last column in the table is the style applied to. |
| [showTableStyleRowStripes](#showTableStyleRowStripes--)| boolean | Indicates whether row stripe formatting is applied to. |
| [showTableStyleColumnStripes](#showTableStyleColumnStripes--)| boolean | Indicates whether column stripe formatting is applied to. |
| [tableStyleType](#tableStyleType--)| TableStyleType | Gets and the built-in table style. |
| [tableStyleName](#tableStyleName--)| string | Gets and sets the table style name. |
| [xmlMap](#xmlMap--)| XmlMap | Readonly. Gets an [XmlMap](../xmlmap/) used for this list. |
| [alternativeText](#alternativeText--)| string | Gets and sets the alternative text. |
| [alternativeDescription](#alternativeDescription--)| string | Gets and sets the alternative description. |

## Methods

| Method | Description |
| --- | --- |
| [resize(number, number, number, number, boolean)](#resize-number-number-number-number-boolean-)| Resize the range of the list object. |
| [putCellValue(number, number, VObject)](#putCellValue-number-number-vobject-)| Put the value to the cell. |
| [putCellValue(number, number, VObject, boolean)](#putCellValue-number-number-vobject-boolean-)| Put the value to the cell. |
| [putCellFormula(number, number, string)](#putCellFormula-number-number-string-)| Put the formula to the cell in the table. |
| [putCellFormula(number, number, string, boolean)](#putCellFormula-number-number-string-boolean-)| Put the formula to the cell in the table. |
| [updateColumnName()](#updateColumnName--)| Updates all list columns' name to cells in the table. |
| [removeAutoFilter()](#removeAutoFilter--)| Removes auto filter which is applied to this table. |
| [filter()](#filter--)| Filter the table. |
| [applyStyleToRange()](#applyStyleToRange--)| Apply the table style to the range. |
| [convertToRange()](#convertToRange--)| Convert the table to range. |
| [convertToRange(TableToRangeOptions)](#convertToRange-tabletorangeoptions-)| Convert the table to range. |


### startRow {#startRow--}

Readonly. Gets the start row of the range.

```javascript
startRow : number;
```


### startColumn {#startColumn--}

Readonly. Gets the start column of the range.

```javascript
startColumn : number;
```


### endRow {#endRow--}

Readonly. Gets the end  row of the range.

```javascript
endRow : number;
```


### endColumn {#endColumn--}

Readonly. Gets the end column of the range.

```javascript
endColumn : number;
```


### listColumns {#listColumns--}

Readonly. Gets the [ListColumn](../listcolumn/) list of this table.

```javascript
listColumns : ListColumnCollection;
```


### showHeaderRow {#showHeaderRow--}

Gets and sets whether this Table shows header row.

```javascript
showHeaderRow : boolean;
```


### showTotals {#showTotals--}

Gets and sets whether this TAble shows total row.

```javascript
showTotals : boolean;
```


### dataRange {#dataRange--}

Readonly. Gets the data range of the Table.

```javascript
dataRange : Range;
```


### queryTable {#queryTable--}

Readonly. Gets the linked QueryTable.

```javascript
queryTable : QueryTable;
```


### dataSourceType {#dataSourceType--}

Readonly. Gets the data source type of the table.

```javascript
dataSourceType : TableDataSourceType;
```


### hasAutoFilter {#hasAutoFilter--}

Indicates whether auto filter is applied to this table.

```javascript
hasAutoFilter : boolean;
```


### autoFilter {#autoFilter--}

Readonly. Gets auto filter of this table.

```javascript
autoFilter : AutoFilter;
```


**Remarks**

It works only when [HasAutoFilter](../hasautofilter/) is false.

### displayName {#displayName--}

Gets and sets the display name of the table.

```javascript
displayName : string;
```


### comment {#comment--}

Gets and sets the comment of the table.

```javascript
comment : string;
```


### showTableStyleFirstColumn {#showTableStyleFirstColumn--}

Indicates whether the first column in the table is the style applied to.

```javascript
showTableStyleFirstColumn : boolean;
```


### showTableStyleLastColumn {#showTableStyleLastColumn--}

Indicates whether the last column in the table is the style applied to.

```javascript
showTableStyleLastColumn : boolean;
```


### showTableStyleRowStripes {#showTableStyleRowStripes--}

Indicates whether row stripe formatting is applied to.

```javascript
showTableStyleRowStripes : boolean;
```


### showTableStyleColumnStripes {#showTableStyleColumnStripes--}

Indicates whether column stripe formatting is applied to.

```javascript
showTableStyleColumnStripes : boolean;
```


### tableStyleType {#tableStyleType--}

Gets and the built-in table style.

```javascript
tableStyleType : TableStyleType;
```


### tableStyleName {#tableStyleName--}

Gets and sets the table style name.

```javascript
tableStyleName : string;
```


### xmlMap {#xmlMap--}

Readonly. Gets an [XmlMap](../xmlmap/) used for this list.

```javascript
xmlMap : XmlMap;
```


### alternativeText {#alternativeText--}

Gets and sets the alternative text.

```javascript
alternativeText : string;
```


### alternativeDescription {#alternativeDescription--}

Gets and sets the alternative description.

```javascript
alternativeDescription : string;
```


### resize(number, number, number, number, boolean) {#resize-number-number-number-number-boolean-}

Resize the range of the list object.

```javascript
resize(startRow: number, startColumn: number, endRow: number, endColumn: number, hasHeaders: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The start row index of the new range. |
| startColumn | number | The start column index of the new range. |
| endRow | number | The end row index of the new range. |
| endColumn | number | The end column index of the new range. |
| hasHeaders | boolean | Whether this table has headers. |

### putCellValue(number, number, VObject) {#putCellValue-number-number-vobject-}

Put the value to the cell.

```javascript
putCellValue(rowOffset: number, columnOffset: number, value: VObject) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | The row offset in the table. |
| columnOffset | number | The column offset in the table. |
| value | VObject | The cell value. |

### putCellValue(number, number, VObject, boolean) {#putCellValue-number-number-vobject-boolean-}

Put the value to the cell.

```javascript
putCellValue(rowOffset: number, columnOffset: number, value: VObject, isTotalsRowLabel: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | The row offset in the table. |
| columnOffset | number | The column offset in the table. |
| value | VObject | The cell value. |
| isTotalsRowLabel | boolean | Indicates whether it is a label for total row,only works for total row.         /// If False and this row is total row, a new row will be inserted. |

### putCellFormula(number, number, string) {#putCellFormula-number-number-string-}

Put the formula to the cell in the table.

```javascript
putCellFormula(rowOffset: number, columnOffset: number, formula: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | The row offset in the table. |
| columnOffset | number | The column offset in the table. |
| formula | string | The formula of the cell. |

### putCellFormula(number, number, string, boolean) {#putCellFormula-number-number-string-boolean-}

Put the formula to the cell in the table.

```javascript
putCellFormula(rowOffset: number, columnOffset: number, formula: string, isTotalsRowFormula: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | The row offset in the table. |
| columnOffset | number | The column offset in the table. |
| formula | string | The formula of the cell. |
| isTotalsRowFormula | boolean |  |

### updateColumnName() {#updateColumnName--}

Updates all list columns' name to cells in the table.

```javascript
updateColumnName() : void;
```


**Remarks**

The value of the cells in the header row of the table must be same as the name of the ListColumn; Cell.PutValue do not auto modify the name of the ListColumn for performance.

### removeAutoFilter() {#removeAutoFilter--}

Removes auto filter which is applied to this table.

```javascript
removeAutoFilter() : void;
```


### filter() {#filter--}

Filter the table.

```javascript
filter() : AutoFilter;
```


**Returns**

[AutoFilter](../autofilter/)

**Remarks**

NOTE: This member is now obsolete. Instead,please set ListObject.HasAutoFilter property. This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### applyStyleToRange() {#applyStyleToRange--}

Apply the table style to the range.

```javascript
applyStyleToRange() : void;
```


### convertToRange() {#convertToRange--}

Convert the table to range.

```javascript
convertToRange() : void;
```


### convertToRange(TableToRangeOptions) {#convertToRange-tabletorangeoptions-}

Convert the table to range.

```javascript
convertToRange(options: TableToRangeOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [TableToRangeOptions](../tabletorangeoptions/) | the options when converting table to range. |


