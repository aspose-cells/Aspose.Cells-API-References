##ListObject
Represents a list object on a worksheet. The ListObject object is a member of the ListObjects collection. The ListObjects collection contains all the list objects on a worksheet.
## ListObject class
Represents a list object on a worksheet. The ListObject object is a member of the ListObjects collection. The ListObjects collection contains all the list objects on a worksheet.
```javascript
class ListObject;
```
### Example
```javascript
const { Workbook, CellsHelper, TotalsCalculation } = require("aspose.cells.node");
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
workbook.save("output/Book1.xlsx");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [startRow](#startRow--)| number | Readonly. Gets the start row of the range. |
| [startColumn](#startColumn--)| number | Readonly. Gets the start column of the range. |
| [endRow](#endRow--)| number | Readonly. Gets the end  row of the range. |
| [endColumn](#endColumn--)| number | Readonly. Gets the end column of the range. |
| [listColumns](#listColumns--)| ListColumnCollection | Readonly. Gets ListColumns of the ListObject. |
| [showHeaderRow](#showHeaderRow--)| boolean | Gets and sets whether this ListObject show header row. |
| [showTotals](#showTotals--)| boolean | Gets and sets whether this ListObject show total row. |
| [dataRange](#dataRange--)| Range | Readonly. Gets the data range of the ListObject. |
| [queryTable](#queryTable--)| QueryTable | Readonly. Gets the linked QueryTable. |
| [dataSourceType](#dataSourceType--)| TableDataSourceType | Readonly. Gets the data source type of the table. |
| [autoFilter](#autoFilter--)| AutoFilter | Readonly. Gets auto filter. |
| [displayName](#displayName--)| string | Gets and sets the display name. |
| [comment](#comment--)| string | Gets and sets the comment of the table. |
| [showTableStyleFirstColumn](#showTableStyleFirstColumn--)| boolean | Indicates whether the first column in the table should have the style applied. |
| [showTableStyleLastColumn](#showTableStyleLastColumn--)| boolean | Indicates whether the last column in the table should have the style applied. |
| [showTableStyleRowStripes](#showTableStyleRowStripes--)| boolean | Indicates whether row stripe formatting is applied. |
| [showTableStyleColumnStripes](#showTableStyleColumnStripes--)| boolean | Indicates whether column stripe formatting is applied. |
| [tableStyleType](#tableStyleType--)| TableStyleType | Gets and the built-in table style. |
| [tableStyleName](#tableStyleName--)| string | Gets and sets the table style name. |
| [xmlMap](#xmlMap--)| XmlMap | Readonly. Gets an [XmlMap](../xmlmap/) used for this list. |
| [alternativeText](#alternativeText--)| string | Gets and sets the alternative text. |
| [alternativeDescription](#alternativeDescription--)| string | Gets and sets the alternative description. |
## Methods
| Method | Description |
| --- | --- |
| [getStartRow()](#getStartRow--)| <b>@deprecated.</b> Please use the 'startRow' property instead. Gets the start row of the range. |
| [getStartColumn()](#getStartColumn--)| <b>@deprecated.</b> Please use the 'startColumn' property instead. Gets the start column of the range. |
| [getEndRow()](#getEndRow--)| <b>@deprecated.</b> Please use the 'endRow' property instead. Gets the end  row of the range. |
| [getEndColumn()](#getEndColumn--)| <b>@deprecated.</b> Please use the 'endColumn' property instead. Gets the end column of the range. |
| [getListColumns()](#getListColumns--)| <b>@deprecated.</b> Please use the 'listColumns' property instead. Gets ListColumns of the ListObject. |
| [getShowHeaderRow()](#getShowHeaderRow--)| <b>@deprecated.</b> Please use the 'showHeaderRow' property instead. Gets and sets whether this ListObject show header row. |
| [setShowHeaderRow(boolean)](#setShowHeaderRow-boolean-)| <b>@deprecated.</b> Please use the 'showHeaderRow' property instead. Gets and sets whether this ListObject show header row. |
| [getShowTotals()](#getShowTotals--)| <b>@deprecated.</b> Please use the 'showTotals' property instead. Gets and sets whether this ListObject show total row. |
| [setShowTotals(boolean)](#setShowTotals-boolean-)| <b>@deprecated.</b> Please use the 'showTotals' property instead. Gets and sets whether this ListObject show total row. |
| [getDataRange()](#getDataRange--)| <b>@deprecated.</b> Please use the 'dataRange' property instead. Gets the data range of the ListObject. |
| [getQueryTable()](#getQueryTable--)| <b>@deprecated.</b> Please use the 'queryTable' property instead. Gets the linked QueryTable. |
| [getDataSourceType()](#getDataSourceType--)| <b>@deprecated.</b> Please use the 'dataSourceType' property instead. Gets the data source type of the table. |
| [getAutoFilter()](#getAutoFilter--)| <b>@deprecated.</b> Please use the 'autoFilter' property instead. Gets auto filter. |
| [getDisplayName()](#getDisplayName--)| <b>@deprecated.</b> Please use the 'displayName' property instead. Gets and sets the display name. |
| [setDisplayName(string)](#setDisplayName-string-)| <b>@deprecated.</b> Please use the 'displayName' property instead. Gets and sets the display name. |
| [getComment()](#getComment--)| <b>@deprecated.</b> Please use the 'comment' property instead. Gets and sets the comment of the table. |
| [setComment(string)](#setComment-string-)| <b>@deprecated.</b> Please use the 'comment' property instead. Gets and sets the comment of the table. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--)| <b>@deprecated.</b> Please use the 'showTableStyleFirstColumn' property instead. Indicates whether the first column in the table should have the style applied. |
| [setShowTableStyleFirstColumn(boolean)](#setShowTableStyleFirstColumn-boolean-)| <b>@deprecated.</b> Please use the 'showTableStyleFirstColumn' property instead. Indicates whether the first column in the table should have the style applied. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--)| <b>@deprecated.</b> Please use the 'showTableStyleLastColumn' property instead. Indicates whether the last column in the table should have the style applied. |
| [setShowTableStyleLastColumn(boolean)](#setShowTableStyleLastColumn-boolean-)| <b>@deprecated.</b> Please use the 'showTableStyleLastColumn' property instead. Indicates whether the last column in the table should have the style applied. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--)| <b>@deprecated.</b> Please use the 'showTableStyleRowStripes' property instead. Indicates whether row stripe formatting is applied. |
| [setShowTableStyleRowStripes(boolean)](#setShowTableStyleRowStripes-boolean-)| <b>@deprecated.</b> Please use the 'showTableStyleRowStripes' property instead. Indicates whether row stripe formatting is applied. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--)| <b>@deprecated.</b> Please use the 'showTableStyleColumnStripes' property instead. Indicates whether column stripe formatting is applied. |
| [setShowTableStyleColumnStripes(boolean)](#setShowTableStyleColumnStripes-boolean-)| <b>@deprecated.</b> Please use the 'showTableStyleColumnStripes' property instead. Indicates whether column stripe formatting is applied. |
| [getTableStyleType()](#getTableStyleType--)| <b>@deprecated.</b> Please use the 'tableStyleType' property instead. Gets and the built-in table style. |
| [setTableStyleType(TableStyleType)](#setTableStyleType-tablestyletype-)| <b>@deprecated.</b> Please use the 'tableStyleType' property instead. Gets and the built-in table style. |
| [getTableStyleName()](#getTableStyleName--)| <b>@deprecated.</b> Please use the 'tableStyleName' property instead. Gets and sets the table style name. |
| [setTableStyleName(string)](#setTableStyleName-string-)| <b>@deprecated.</b> Please use the 'tableStyleName' property instead. Gets and sets the table style name. |
| [getXmlMap()](#getXmlMap--)| <b>@deprecated.</b> Please use the 'xmlMap' property instead. Gets an [XmlMap](../xmlmap/) used for this list. |
| [getAlternativeText()](#getAlternativeText--)| <b>@deprecated.</b> Please use the 'alternativeText' property instead. Gets and sets the alternative text. |
| [setAlternativeText(string)](#setAlternativeText-string-)| <b>@deprecated.</b> Please use the 'alternativeText' property instead. Gets and sets the alternative text. |
| [getAlternativeDescription()](#getAlternativeDescription--)| <b>@deprecated.</b> Please use the 'alternativeDescription' property instead. Gets and sets the alternative description. |
| [setAlternativeDescription(string)](#setAlternativeDescription-string-)| <b>@deprecated.</b> Please use the 'alternativeDescription' property instead. Gets and sets the alternative description. |
| [resize(number, number, number, number, boolean)](#resize-number-number-number-number-boolean-)| Resize the range of the list object. |
| [putCellValue(number, number, Object)](#putCellValue-number-number-object-)| Put the value to the cell. |
| [putCellValue(number, number, Object, boolean)](#putCellValue-number-number-object-boolean-)| Put the value to the cell. |
| [putCellFormula(number, number, string)](#putCellFormula-number-number-string-)| Put the formula to the cell in the table. |
| [putCellFormula(number, number, string, boolean)](#putCellFormula-number-number-string-boolean-)| Put the formula to the cell in the table. |
| [updateColumnName()](#updateColumnName--)| Updates all list columns' name from the worksheet. |
| [filter()](#filter--)| Filter the table. |
| [applyStyleToRange()](#applyStyleToRange--)| Apply the table style to the range. |
| [convertToRange()](#convertToRange--)| Convert the table to range. |
| [convertToRange(TableToRangeOptions)](#convertToRange-tabletorangeoptions-)| Convert the table to range. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
Readonly. Gets ListColumns of the ListObject.
```javascript
listColumns : ListColumnCollection;
```
### showHeaderRow {#showHeaderRow--}
Gets and sets whether this ListObject show header row.
```javascript
showHeaderRow : boolean;
```
### showTotals {#showTotals--}
Gets and sets whether this ListObject show total row.
```javascript
showTotals : boolean;
```
### dataRange {#dataRange--}
Readonly. Gets the data range of the ListObject.
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
### autoFilter {#autoFilter--}
Readonly. Gets auto filter.
```javascript
autoFilter : AutoFilter;
```
### displayName {#displayName--}
Gets and sets the display name.
```javascript
displayName : string;
```
### comment {#comment--}
Gets and sets the comment of the table.
```javascript
comment : string;
```
### showTableStyleFirstColumn {#showTableStyleFirstColumn--}
Indicates whether the first column in the table should have the style applied.
```javascript
showTableStyleFirstColumn : boolean;
```
### showTableStyleLastColumn {#showTableStyleLastColumn--}
Indicates whether the last column in the table should have the style applied.
```javascript
showTableStyleLastColumn : boolean;
```
### showTableStyleRowStripes {#showTableStyleRowStripes--}
Indicates whether row stripe formatting is applied.
```javascript
showTableStyleRowStripes : boolean;
```
### showTableStyleColumnStripes {#showTableStyleColumnStripes--}
Indicates whether column stripe formatting is applied.
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
### getStartRow() {#getStartRow--}
```javascript
getStartRow() : number;
```
### getStartColumn() {#getStartColumn--}
```javascript
getStartColumn() : number;
```
### getEndRow() {#getEndRow--}
```javascript
getEndRow() : number;
```
### getEndColumn() {#getEndColumn--}
```javascript
getEndColumn() : number;
```
### getListColumns() {#getListColumns--}
```javascript
getListColumns() : ListColumnCollection;
```
**Returns**
[ListColumnCollection](../listcolumncollection/)
### getShowHeaderRow() {#getShowHeaderRow--}
```javascript
getShowHeaderRow() : boolean;
```
### setShowHeaderRow(boolean) {#setShowHeaderRow-boolean-}
```javascript
setShowHeaderRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowTotals() {#getShowTotals--}
```javascript
getShowTotals() : boolean;
```
### setShowTotals(boolean) {#setShowTotals-boolean-}
```javascript
setShowTotals(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDataRange() {#getDataRange--}
```javascript
getDataRange() : Range;
```
**Returns**
[Range](../range/)
### getQueryTable() {#getQueryTable--}
```javascript
getQueryTable() : QueryTable;
```
**Returns**
[QueryTable](../querytable/)
### getDataSourceType() {#getDataSourceType--}
```javascript
getDataSourceType() : TableDataSourceType;
```
**Returns**
[TableDataSourceType](../tabledatasourcetype/)
### getAutoFilter() {#getAutoFilter--}
```javascript
getAutoFilter() : AutoFilter;
```
**Returns**
[AutoFilter](../autofilter/)
### getDisplayName() {#getDisplayName--}
```javascript
getDisplayName() : string;
```
### setDisplayName(string) {#setDisplayName-string-}
```javascript
setDisplayName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getComment() {#getComment--}
```javascript
getComment() : string;
```
### setComment(string) {#setComment-string-}
```javascript
setComment(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```javascript
getShowTableStyleFirstColumn() : boolean;
```
### setShowTableStyleFirstColumn(boolean) {#setShowTableStyleFirstColumn-boolean-}
```javascript
setShowTableStyleFirstColumn(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```javascript
getShowTableStyleLastColumn() : boolean;
```
### setShowTableStyleLastColumn(boolean) {#setShowTableStyleLastColumn-boolean-}
```javascript
setShowTableStyleLastColumn(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```javascript
getShowTableStyleRowStripes() : boolean;
```
### setShowTableStyleRowStripes(boolean) {#setShowTableStyleRowStripes-boolean-}
```javascript
setShowTableStyleRowStripes(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```javascript
getShowTableStyleColumnStripes() : boolean;
```
### setShowTableStyleColumnStripes(boolean) {#setShowTableStyleColumnStripes-boolean-}
```javascript
setShowTableStyleColumnStripes(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getTableStyleType() {#getTableStyleType--}
```javascript
getTableStyleType() : TableStyleType;
```
**Returns**
[TableStyleType](../tablestyletype/)
### setTableStyleType(TableStyleType) {#setTableStyleType-tablestyletype-}
```javascript
setTableStyleType(value: TableStyleType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TableStyleType](../tablestyletype/) | The value to set. |
### getTableStyleName() {#getTableStyleName--}
```javascript
getTableStyleName() : string;
```
### setTableStyleName(string) {#setTableStyleName-string-}
```javascript
setTableStyleName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getXmlMap() {#getXmlMap--}
```javascript
getXmlMap() : XmlMap;
```
**Returns**
[XmlMap](../xmlmap/)
### getAlternativeText() {#getAlternativeText--}
```javascript
getAlternativeText() : string;
```
### setAlternativeText(string) {#setAlternativeText-string-}
```javascript
setAlternativeText(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getAlternativeDescription() {#getAlternativeDescription--}
```javascript
getAlternativeDescription() : string;
```
### setAlternativeDescription(string) {#setAlternativeDescription-string-}
```javascript
setAlternativeDescription(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
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
### putCellValue(number, number, Object) {#putCellValue-number-number-object-}
Put the value to the cell.
```javascript
putCellValue(rowOffset: number, columnOffset: number, value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | The row offset in the table. |
| columnOffset | number | The column offset in the table. |
| value | Object | The cell value. |
### putCellValue(number, number, Object, boolean) {#putCellValue-number-number-object-boolean-}
Put the value to the cell.
```javascript
putCellValue(rowOffset: number, columnOffset: number, value: Object, isTotalsRowLabel: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | The row offset in the table. |
| columnOffset | number | The column offset in the table. |
| value | Object | The cell value. |
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
Updates all list columns' name from the worksheet.
```javascript
updateColumnName() : void;
```
**Remarks**
The value of the cells in the header row of the table must be same as the name of the ListColumn; Cell.PutValue do not auto modify the name of the ListColumn for performance.
### filter() {#filter--}
Filter the table.
```javascript
filter() : AutoFilter;
```
**Returns**
[AutoFilter](../autofilter/)
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
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
