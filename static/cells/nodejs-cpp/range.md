##Range
Encapsulates the object that represents a range of cells within a spreadsheet.
## Range class
Encapsulates the object that represents a range of cells within a spreadsheet.
```javascript
class Range;
```
### Remarks
The Range class denotes a region of Excel spreadsheet. With this, you can format and set value of the range. And you can simply copy range of Excel too.
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [currentRegion](#currentRegion--)| Range | Readonly. Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns. |
| [hyperlinks](#hyperlinks--)| Hyperlink[] | Readonly. Gets all hyperlink in the range. |
| [rowCount](#rowCount--)| number | Readonly. Gets the count of rows in the range. |
| [columnCount](#columnCount--)| number | Readonly. Gets the count of columns in the range. |
| [name](#name--)| string | Gets or sets the name of the range. |
| [refersTo](#refersTo--)| string | Readonly. Gets the range's refers to. |
| [address](#address--)| string | Readonly. Gets address of the range. |
| [left](#left--)| number | Readonly. Gets the distance, in points, from the left edge of column A to the left edge of the range. |
| [top](#top--)| number | Readonly. Gets the distance, in points, from the top edge of row 1 to the top edge of the range. |
| [width](#width--)| number | Readonly. Gets the width of a range in points. |
| [height](#height--)| number | Readonly. Gets the width of a range in points. |
| [firstRow](#firstRow--)| number | Readonly. Gets the index of the first row of the range. |
| [firstColumn](#firstColumn--)| number | Readonly. Gets the index of the first column of the range. |
| [value](#value--)| Object | Gets and sets the value of the range. |
| [columnWidth](#columnWidth--)| number | Sets or gets the column width of this range |
| [rowHeight](#rowHeight--)| number | Sets or gets the height of rows in this range |
| [entireColumn](#entireColumn--)| Range | Readonly. Gets a Range object that represents the entire column (or columns) that contains the specified range. |
| [entireRow](#entireRow--)| Range | Readonly. Gets a Range object that represents the entire row (or rows) that contains the specified range. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the [Worksheet](../worksheet/)object which contains this range. |
## Methods
| Method | Description |
| --- | --- |
| [get(number, number)](#get-number-number-)| Gets [Cell](../cell/) object in this range. |
| [getCurrentRegion()](#getCurrentRegion--)| <b>@deprecated.</b> Please use the 'currentRegion' property instead. Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns. |
| [getHyperlinks()](#getHyperlinks--)| <b>@deprecated.</b> Please use the 'hyperlinks' property instead. Gets all hyperlink in the range. |
| [getRowCount()](#getRowCount--)| <b>@deprecated.</b> Please use the 'rowCount' property instead. Gets the count of rows in the range. |
| [getColumnCount()](#getColumnCount--)| <b>@deprecated.</b> Please use the 'columnCount' property instead. Gets the count of columns in the range. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets or sets the name of the range. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets or sets the name of the range. |
| [getRefersTo()](#getRefersTo--)| <b>@deprecated.</b> Please use the 'refersTo' property instead. Gets the range's refers to. |
| [getAddress()](#getAddress--)| <b>@deprecated.</b> Please use the 'address' property instead. Gets address of the range. |
| [getLeft()](#getLeft--)| <b>@deprecated.</b> Please use the 'left' property instead. Gets the distance, in points, from the left edge of column A to the left edge of the range. |
| [getTop()](#getTop--)| <b>@deprecated.</b> Please use the 'top' property instead. Gets the distance, in points, from the top edge of row 1 to the top edge of the range. |
| [getWidth()](#getWidth--)| <b>@deprecated.</b> Please use the 'width' property instead. Gets the width of a range in points. |
| [getHeight()](#getHeight--)| <b>@deprecated.</b> Please use the 'height' property instead. Gets the width of a range in points. |
| [getFirstRow()](#getFirstRow--)| <b>@deprecated.</b> Please use the 'firstRow' property instead. Gets the index of the first row of the range. |
| [getFirstColumn()](#getFirstColumn--)| <b>@deprecated.</b> Please use the 'firstColumn' property instead. Gets the index of the first column of the range. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets and sets the value of the range. |
| [setValue(Object)](#setValue-object-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets and sets the value of the range. |
| [getColumnWidth()](#getColumnWidth--)| <b>@deprecated.</b> Please use the 'columnWidth' property instead. Sets or gets the column width of this range |
| [setColumnWidth(number)](#setColumnWidth-number-)| <b>@deprecated.</b> Please use the 'columnWidth' property instead. Sets or gets the column width of this range |
| [getRowHeight()](#getRowHeight--)| <b>@deprecated.</b> Please use the 'rowHeight' property instead. Sets or gets the height of rows in this range |
| [setRowHeight(number)](#setRowHeight-number-)| <b>@deprecated.</b> Please use the 'rowHeight' property instead. Sets or gets the height of rows in this range |
| [getEntireColumn()](#getEntireColumn--)| <b>@deprecated.</b> Please use the 'entireColumn' property instead. Gets a Range object that represents the entire column (or columns) that contains the specified range. |
| [getEntireRow()](#getEntireRow--)| <b>@deprecated.</b> Please use the 'entireRow' property instead. Gets a Range object that represents the entire row (or rows) that contains the specified range. |
| [getWorksheet()](#getWorksheet--)| <b>@deprecated.</b> Please use the 'worksheet' property instead. Gets the [Worksheet](../worksheet/)object which contains this range. |
| [autoFill(Range)](#autoFill-range-)| Automaticall fill the target range. |
| [autoFill(Range, AutoFillType)](#autoFill-range-autofilltype-)| Automaticall fill the target range. |
| [addHyperlink(string, string, string)](#addHyperlink-string-string-string-)| Adds a hyperlink to a specified cell or a range of cells. |
| [getEnumerator()](#getEnumerator--)| Gets the enumerator for cells in this Range. |
| [isIntersect(Range)](#isIntersect-range-)| Indicates whether the range is intersect. |
| [intersect(Range)](#intersect-range-)| Returns a [Range](../range/) object that represents the rectangular intersection of two ranges. |
| [unionRang(Range)](#unionRang-range-)| Returns the union result of two ranges. |
| [unionRanges(Range[])](#unionRanges-rangearray-)| Returns the union result of two ranges. |
| [isBlank()](#isBlank--)| Indicates whether the range contains values. |
| [merge()](#merge--)| Combines a range of cells into a single cell. |
| [unMerge()](#unMerge--)| Unmerges merged cells of this range. |
| [putValue(string, boolean, boolean)](#putValue-string-boolean-boolean-)| Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [setStyle(Style, boolean)](#setStyle-style-boolean-)| Apply the cell style. |
| [setStyle(Style)](#setStyle-style-)| Sets the style of the range. |
| [applyStyle(Style, StyleFlag)](#applyStyle-style-styleflag-)| Applies formats for a whole range. |
| [setOutlineBorders(CellBorderType, CellsColor)](#setOutlineBorders-cellbordertype-cellscolor-)| Sets the outline borders around a range of cells with same border style and color. |
| [setOutlineBorders(CellBorderType, Color)](#setOutlineBorders-cellbordertype-color-)| Sets the outline borders around a range of cells with same border style and color. |
| [setOutlineBorders(CellBorderType[], Color[])](#setOutlineBorders-cellbordertypearray-colorarray-)| Sets out line borders around a range of cells. |
| [setOutlineBorder(BorderType, CellBorderType, CellsColor)](#setOutlineBorder-bordertype-cellbordertype-cellscolor-)| Sets outline border around a range of cells. |
| [setOutlineBorder(BorderType, CellBorderType, Color)](#setOutlineBorder-bordertype-cellbordertype-color-)| Sets outline border around a range of cells. |
| [setInsideBorders(BorderType, CellBorderType, CellsColor)](#setInsideBorders-bordertype-cellbordertype-cellscolor-)| Set inside borders of the range. |
| [moveTo(number, number)](#moveTo-number-number-)| Move the current range to the dest range. |
| [copyData(Range)](#copyData-range-)| Copies cell data (including formulas) from a source range. |
| [copyValue(Range)](#copyValue-range-)| Copies cell value from a source range. |
| [copyStyle(Range)](#copyStyle-range-)| Copies style settings from a source range. |
| [copy(Range, PasteOptions)](#copy-range-pasteoptions-)| Copying the range with paste special options. |
| [copy(Range)](#copy-range-)| Copies data (including formulas), formatting, drawing objects etc. from a source range. |
| [transpose()](#transpose--)| Transpose (rotate) data from rows to columns or vice versa. |
| [getCellOrNull(number, number)](#getCellOrNull-number-number-)| Gets [Cell](../cell/) object or null in this range. |
| [getOffset(number, number)](#getOffset-number-number-)| Gets [Range](../range/) range by offset. |
| [toImage(ImageOrPrintOptions)](#toImage-imageorprintoptions-)| Converts the range to image. |
| [toJson(JsonSaveOptions)](#toJson-jsonsaveoptions-)| Convert the range to JSON value. |
| [toHtml(HtmlSaveOptions)](#toHtml-htmlsaveoptions-)| Convert the range to html . |
| [clear()](#clear--)| Clears this range. |
| [clearContents()](#clearContents--)| Clears the contents of this range. |
| [clearFormats()](#clearFormats--)| Clears the formats of this range. |
| [clearComments()](#clearComments--)| Clears the comments of this range. |
| [clearHyperlinks(boolean)](#clearHyperlinks-boolean-)| Only removes hyperlinks. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [toString()](#toString--)| Returns a string represents the current Range object. |
### currentRegion {#currentRegion--}
Readonly. Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns.
```javascript
currentRegion : Range;
```
### hyperlinks {#hyperlinks--}
Readonly. Gets all hyperlink in the range.
```javascript
hyperlinks : Hyperlink[];
```
### rowCount {#rowCount--}
Readonly. Gets the count of rows in the range.
```javascript
rowCount : number;
```
### columnCount {#columnCount--}
Readonly. Gets the count of columns in the range.
```javascript
columnCount : number;
```
### name {#name--}
Gets or sets the name of the range.
```javascript
name : string;
```
**Remarks**
Named range is supported. For example, <p>range.Name = "Sheet1!MyRange";
### refersTo {#refersTo--}
Readonly. Gets the range's refers to.
```javascript
refersTo : string;
```
### address {#address--}
Readonly. Gets address of the range.
```javascript
address : string;
```
### left {#left--}
Readonly. Gets the distance, in points, from the left edge of column A to the left edge of the range.
```javascript
left : number;
```
### top {#top--}
Readonly. Gets the distance, in points, from the top edge of row 1 to the top edge of the range.
```javascript
top : number;
```
### width {#width--}
Readonly. Gets the width of a range in points.
```javascript
width : number;
```
### height {#height--}
Readonly. Gets the width of a range in points.
```javascript
height : number;
```
### firstRow {#firstRow--}
Readonly. Gets the index of the first row of the range.
```javascript
firstRow : number;
```
### firstColumn {#firstColumn--}
Readonly. Gets the index of the first column of the range.
```javascript
firstColumn : number;
```
### value {#value--}
Gets and sets the value of the range.
```javascript
value : Object;
```
**Remarks**
If the range contains multiple cells, the returned/applied object should be a two-dimension [Array](../array/) object.
### columnWidth {#columnWidth--}
Sets or gets the column width of this range
```javascript
columnWidth : number;
```
### rowHeight {#rowHeight--}
Sets or gets the height of rows in this range
```javascript
rowHeight : number;
```
### entireColumn {#entireColumn--}
Readonly. Gets a Range object that represents the entire column (or columns) that contains the specified range.
```javascript
entireColumn : Range;
```
### entireRow {#entireRow--}
Readonly. Gets a Range object that represents the entire row (or rows) that contains the specified range.
```javascript
entireRow : Range;
```
### worksheet {#worksheet--}
Readonly. Gets the [Worksheet](../worksheet/)object which contains this range.
```javascript
worksheet : Worksheet;
```
### get(number, number) {#get-number-number-}
Gets [Cell](../cell/) object in this range.
```javascript
get(rowOffset: number, columnOffset: number) : Cell;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | Row offset in this range, zero based. |
| columnOffset | number | Column offset in this range, zero based. |
**Returns**
[Cell](../cell/) object.
### getCurrentRegion() {#getCurrentRegion--}
```javascript
getCurrentRegion() : Range;
```
**Returns**
[Range](../range/)
### getHyperlinks() {#getHyperlinks--}
```javascript
getHyperlinks() : Hyperlink[];
```
**Returns**
[Hyperlink](../hyperlink/)[]
### getRowCount() {#getRowCount--}
```javascript
getRowCount() : number;
```
### getColumnCount() {#getColumnCount--}
```javascript
getColumnCount() : number;
```
### getName() {#getName--}
```javascript
getName() : string;
```
**Remarks**
Named range is supported. For example, <p>range.Name = "Sheet1!MyRange";
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
Named range is supported. For example, <p>range.Name = "Sheet1!MyRange";
### getRefersTo() {#getRefersTo--}
```javascript
getRefersTo() : string;
```
### getAddress() {#getAddress--}
```javascript
getAddress() : string;
```
### getLeft() {#getLeft--}
```javascript
getLeft() : number;
```
### getTop() {#getTop--}
```javascript
getTop() : number;
```
### getWidth() {#getWidth--}
```javascript
getWidth() : number;
```
### getHeight() {#getHeight--}
```javascript
getHeight() : number;
```
### getFirstRow() {#getFirstRow--}
```javascript
getFirstRow() : number;
```
### getFirstColumn() {#getFirstColumn--}
```javascript
getFirstColumn() : number;
```
### getValue() {#getValue--}
```javascript
getValue() : Object;
```
**Remarks**
If the range contains multiple cells, the returned/applied object should be a two-dimension [Array](../array/) object.
### setValue(Object) {#setValue-object-}
```javascript
setValue(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
**Remarks**
If the range contains multiple cells, the returned/applied object should be a two-dimension [Array](../array/) object.
### getColumnWidth() {#getColumnWidth--}
```javascript
getColumnWidth() : number;
```
### setColumnWidth(number) {#setColumnWidth-number-}
```javascript
setColumnWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRowHeight() {#getRowHeight--}
```javascript
getRowHeight() : number;
```
### setRowHeight(number) {#setRowHeight-number-}
```javascript
setRowHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getEntireColumn() {#getEntireColumn--}
```javascript
getEntireColumn() : Range;
```
**Returns**
[Range](../range/)
### getEntireRow() {#getEntireRow--}
```javascript
getEntireRow() : Range;
```
**Returns**
[Range](../range/)
### getWorksheet() {#getWorksheet--}
```javascript
getWorksheet() : Worksheet;
```
**Returns**
[Worksheet](../worksheet/)
### autoFill(Range) {#autoFill-range-}
Automaticall fill the target range.
```javascript
autoFill(target: Range) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| target | [Range](../range/) | the target range. |
### autoFill(Range, AutoFillType) {#autoFill-range-autofilltype-}
Automaticall fill the target range.
```javascript
autoFill(target: Range, autoFillType: AutoFillType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| target | [Range](../range/) | The targed range. |
| autoFillType | [AutoFillType](../autofilltype/) | The auto fill type. |
### addHyperlink(string, string, string) {#addHyperlink-string-string-string-}
Adds a hyperlink to a specified cell or a range of cells.
```javascript
addHyperlink(address: string, textToDisplay: string, screenTip: string) : Hyperlink;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | string | Address of the hyperlink. |
| textToDisplay | string | The text to be displayed for the specified hyperlink. |
| screenTip | string | The screenTip text for the specified hyperlink. |
**Returns**
[Hyperlink](../hyperlink/) object.
### getEnumerator() {#getEnumerator--}
Gets the enumerator for cells in this Range.
```javascript
getEnumerator() : CellEnumerator;
```
**Returns**
The cells enumerator
**Remarks**
When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).
### isIntersect(Range) {#isIntersect-range-}
Indicates whether the range is intersect.
```javascript
isIntersect(range: Range) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | The range. |
**Returns**
Whether the range is intersect.
**Remarks**
If the two ranges area not in the same worksheet ,return false.
### intersect(Range) {#intersect-range-}
Returns a [Range](../range/) object that represents the rectangular intersection of two ranges.
```javascript
intersect(range: Range) : Range;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | The intersecting range. |
**Returns**
Returns a [Range](../range/) object
**Remarks**
If the two ranges are not intersected, returns null.
### unionRang(Range) {#unionRang-range-}
Returns the union result of two ranges.
```javascript
unionRang(range: Range) : Range[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | The range |
**Returns**
The union of two ranges.
**Remarks**
NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This method will be removed 12 months later since May 2024. Aspose apologizes for any inconvenience you may have experienced.
### unionRanges(Range[]) {#unionRanges-rangearray-}
Returns the union result of two ranges.
```javascript
unionRanges(ranges: Range[]) : UnionRange;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ranges | [Range](../range/)[] | The range |
**Returns**
The union of two ranges.
### isBlank() {#isBlank--}
Indicates whether the range contains values.
```javascript
isBlank() : boolean;
```
### merge() {#merge--}
Combines a range of cells into a single cell.
```javascript
merge() : void;
```
**Remarks**
Reference the merged cell via the address of the upper-left cell in the range.
### unMerge() {#unMerge--}
Unmerges merged cells of this range.
```javascript
unMerge() : void;
```
### putValue(string, boolean, boolean) {#putValue-string-boolean-boolean-}
Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.
```javascript
putValue(stringValue: string, isConverted: boolean, setStyle: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | string | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |
### setStyle(Style, boolean) {#setStyle-style-boolean-}
Apply the cell style.
```javascript
setStyle(style: Style, explicitFlag: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The cell style. |
| explicitFlag | boolean | True, only overwriting formatting which is explicitly set. |
### setStyle(Style) {#setStyle-style-}
Sets the style of the range.
```javascript
setStyle(style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The Style object. |
### applyStyle(Style, StyleFlag) {#applyStyle-style-styleflag-}
Applies formats for a whole range.
```javascript
applyStyle(style: Style, flag: StyleFlag) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The style object which will be applied. |
| flag | [StyleFlag](../styleflag/) | Flags which indicates applied formatting properties. |
**Remarks**
Each cell in this range will contains a [Style](../style/) object. So this is a memory-consuming method. Please use it carefully.
### setOutlineBorders(CellBorderType, CellsColor) {#setOutlineBorders-cellbordertype-cellscolor-}
Sets the outline borders around a range of cells with same border style and color.
```javascript
setOutlineBorders(borderStyle: CellBorderType, borderColor: CellsColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | [CellBorderType](../cellbordertype/) | Border style. |
| borderColor | [CellsColor](../cellscolor/) | Border color. |
### setOutlineBorders(CellBorderType, Color) {#setOutlineBorders-cellbordertype-color-}
Sets the outline borders around a range of cells with same border style and color.
```javascript
setOutlineBorders(borderStyle: CellBorderType, borderColor: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | [CellBorderType](../cellbordertype/) | Border style. |
| borderColor | [Color](../color/) | Border color. |
### setOutlineBorders(CellBorderType[], Color[]) {#setOutlineBorders-cellbordertypearray-colorarray-}
Sets out line borders around a range of cells.
```javascript
setOutlineBorders(borderStyles: CellBorderType[], borderColors: Color[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | [CellBorderType](../cellbordertype/)[] | Border styles. |
| borderColors | [Color](../color/)[] | Border colors. |
**Remarks**
Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right
### setOutlineBorder(BorderType, CellBorderType, CellsColor) {#setOutlineBorder-bordertype-cellbordertype-cellscolor-}
Sets outline border around a range of cells.
```javascript
setOutlineBorder(borderEdge: BorderType, borderStyle: CellBorderType, borderColor: CellsColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | [BorderType](../bordertype/) | Border edge. |
| borderStyle | [CellBorderType](../cellbordertype/) | Border style. |
| borderColor | [CellsColor](../cellscolor/) | Border color. |
### setOutlineBorder(BorderType, CellBorderType, Color) {#setOutlineBorder-bordertype-cellbordertype-color-}
Sets outline border around a range of cells.
```javascript
setOutlineBorder(borderEdge: BorderType, borderStyle: CellBorderType, borderColor: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | [BorderType](../bordertype/) | Border edge. |
| borderStyle | [CellBorderType](../cellbordertype/) | Border style. |
| borderColor | [Color](../color/) | Border color. |
### setInsideBorders(BorderType, CellBorderType, CellsColor) {#setInsideBorders-bordertype-cellbordertype-cellscolor-}
Set inside borders of the range.
```javascript
setInsideBorders(borderEdge: BorderType, lineStyle: CellBorderType, borderColor: CellsColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | [BorderType](../bordertype/) | Inside borde type, only can be [BorderType.Vertical](../bordertype.vertical/) and [BorderType.Horizontal](../bordertype.horizontal/). |
| lineStyle | [CellBorderType](../cellbordertype/) | The border style. |
| borderColor | [CellsColor](../cellscolor/) | The color of the border. |
### moveTo(number, number) {#moveTo-number-number-}
Move the current range to the dest range.
```javascript
moveTo(destRow: number, destColumn: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destRow | number | The start row of the dest range. |
| destColumn | number | The start column of the dest range. |
### copyData(Range) {#copyData-range-}
Copies cell data (including formulas) from a source range.
```javascript
copyData(range: Range) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | Source [Range](../range/) object. |
### copyValue(Range) {#copyValue-range-}
Copies cell value from a source range.
```javascript
copyValue(range: Range) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | Source [Range](../range/) object. |
### copyStyle(Range) {#copyStyle-range-}
Copies style settings from a source range.
```javascript
copyStyle(range: Range) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | Source [Range](../range/) object. |
### copy(Range, PasteOptions) {#copy-range-pasteoptions-}
Copying the range with paste special options.
```javascript
copy(range: Range, options: PasteOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | The source range. |
| options | [PasteOptions](../pasteoptions/) | The paste special options. |
### copy(Range) {#copy-range-}
Copies data (including formulas), formatting, drawing objects etc. from a source range.
```javascript
copy(range: Range) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | Source [Range](../range/) object. |
### transpose() {#transpose--}
Transpose (rotate) data from rows to columns or vice versa.
```javascript
transpose() : void;
```
### getCellOrNull(number, number) {#getCellOrNull-number-number-}
Gets [Cell](../cell/) object or null in this range.
```javascript
getCellOrNull(rowOffset: number, columnOffset: number) : Cell;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | Row offset in this range, zero based. |
| columnOffset | number | Column offset in this range, zero based. |
**Returns**
[Cell](../cell/) object.
### getOffset(number, number) {#getOffset-number-number-}
Gets [Range](../range/) range by offset.
```javascript
getOffset(rowOffset: number, columnOffset: number) : Range;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | Row offset in this range, zero based. |
| columnOffset | number | Column offset in this range, zero based. |
**Returns**
[Range](../range/)
### toImage(ImageOrPrintOptions) {#toImage-imageorprintoptions-}
Converts the range to image.
```javascript
toImage(options: ImageOrPrintOptions) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | The options for converting this range to image |
### toJson(JsonSaveOptions) {#toJson-jsonsaveoptions-}
Convert the range to JSON value.
```javascript
toJson(options: JsonSaveOptions) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [JsonSaveOptions](../jsonsaveoptions/) | The options of converting |
### toHtml(HtmlSaveOptions) {#toHtml-htmlsaveoptions-}
Convert the range to html .
```javascript
toHtml(saveOptions: HtmlSaveOptions) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../htmlsaveoptions/) | Options for coverting range to html. |
### clear() {#clear--}
Clears this range.
```javascript
clear() : void;
```
### clearContents() {#clearContents--}
Clears the contents of this range.
```javascript
clearContents() : void;
```
### clearFormats() {#clearFormats--}
Clears the formats of this range.
```javascript
clearFormats() : void;
```
### clearComments() {#clearComments--}
Clears the comments of this range.
```javascript
clearComments() : void;
```
### clearHyperlinks(boolean) {#clearHyperlinks-boolean-}
Only removes hyperlinks.
```javascript
clearHyperlinks(clearFormat: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| clearFormat | boolean | Indicates whether to clear the format of hyperlinks. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### toString() {#toString--}
Returns a string represents the current Range object.
```javascript
toString() : string;
```
