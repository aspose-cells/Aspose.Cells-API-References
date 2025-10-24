##Row
Represents a single row in a worksheet.
## Row class
Represents a single row in a worksheet.
```javascript
class Row;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isBlank](#isBlank--)| boolean | Readonly. Indicates whether the row contains any data |
| [isCollapsed](#isCollapsed--)| boolean | whether the row is collapsed |
| [height](#height--)| number | Gets and sets the row height in unit of Points. |
| [isHidden](#isHidden--)| boolean | Indicates whether the row is hidden. |
| [index](#index--)| number | Readonly. Gets the index of this row. |
| [groupLevel](#groupLevel--)| number | Gets the group level of the row. |
| [isHeightMatched](#isHeightMatched--)| boolean | Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user. |
| [hasCustomStyle](#hasCustomStyle--)| boolean | Readonly. Indicates whether this row has custom style settings(different from the default one inherited from workbook). |
| [firstCell](#firstCell--)| Cell | Readonly. Gets the first cell object in the row. |
| [firstDataCell](#firstDataCell--)| Cell | Readonly. Gets the first non-blank cell in the row. |
| [lastCell](#lastCell--)| Cell | Readonly. Gets the last cell object in the row. |
| [lastDataCell](#lastDataCell--)| Cell | Readonly. Gets the last non-blank cell in the row. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the cell. |
| [getCellByIndex(number)](#getCellByIndex-number-)| Get the cell by specific index in the cells collection of this row. |
| [getEnumerator()](#getEnumerator--)| Gets the cells enumerator |
| [getEnumerator(boolean, boolean)](#getEnumerator-boolean-boolean-)| Gets an enumerator that iterates cells through this row. |
| [getCellOrNull(number)](#getCellOrNull-number-)| Gets the cell or null in the specific index. |
| [getStyle()](#getStyle--)| Gets the style of this row. |
| [setStyle(Style)](#setStyle-style-)| Sets the style of this row. |
| [copySettings(Row, boolean)](#copySettings-row-boolean-)| Copy settings of row, such as style, height, visibility, ...etc. |
| [applyStyle(Style, StyleFlag)](#applyStyle-style-styleflag-)| Applies formats for a whole row. |
| [equals(VObject)](#equals-vobject-)| Checks whether this object refers to the same row with another. |
| [equals(Row)](#equals-row-)| Checks whether this object refers to the same row with another row object. |
### isBlank {#isBlank--}
Readonly. Indicates whether the row contains any data
```javascript
isBlank : boolean;
```
### isCollapsed {#isCollapsed--}
whether the row is collapsed
```javascript
isCollapsed : boolean;
```
### height {#height--}
Gets and sets the row height in unit of Points.
```javascript
height : number;
```
### isHidden {#isHidden--}
Indicates whether the row is hidden.
```javascript
isHidden : boolean;
```
### index {#index--}
Readonly. Gets the index of this row.
```javascript
index : number;
```
### groupLevel {#groupLevel--}
Gets the group level of the row.
```javascript
groupLevel : number;
```
### isHeightMatched {#isHeightMatched--}
Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user.
```javascript
isHeightMatched : boolean;
```
**Remarks**
When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by [Worksheet.AutoFitRows()](../worksheet.autofitrows()/)) to get the same result with what is shown in ms excel when you opening the workbook in it.
### hasCustomStyle {#hasCustomStyle--}
Readonly. Indicates whether this row has custom style settings(different from the default one inherited from workbook).
```javascript
hasCustomStyle : boolean;
```
### firstCell {#firstCell--}
Readonly. Gets the first cell object in the row.
```javascript
firstCell : Cell;
```
### firstDataCell {#firstDataCell--}
Readonly. Gets the first non-blank cell in the row.
```javascript
firstDataCell : Cell;
```
### lastCell {#lastCell--}
Readonly. Gets the last cell object in the row.
```javascript
lastCell : Cell;
```
### lastDataCell {#lastDataCell--}
Readonly. Gets the last non-blank cell in the row.
```javascript
lastDataCell : Cell;
```
### get(number) {#get-number-}
Gets the cell.
```javascript
get(column: number) : Cell;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | The column index |
**Returns**
[Cell](../cell/)
### getCellByIndex(number) {#getCellByIndex-number-}
Get the cell by specific index in the cells collection of this row.
```javascript
getCellByIndex(index: number) : Cell;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index(position) of the cell in the cells collection of this row. |
**Returns**
The Cell object at given position.
**Remarks**
To traverse all cells in sequence without modification, using [GetEnumerator()](../getenumerator()/) will give better performance than using this method to get cell one by one.
### getEnumerator() {#getEnumerator--}
Gets the cells enumerator
```javascript
getEnumerator() : CellEnumerator;
```
**Returns**
The cells enumerator which will traverse all existing cells in this row.
### getEnumerator(boolean, boolean) {#getEnumerator-boolean-boolean-}
Gets an enumerator that iterates cells through this row.
```javascript
getEnumerator(reversed: boolean, sync: boolean) : CellEnumerator;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| reversed | boolean | whether enumerate cells in reversed order |
| sync | boolean | whether the returned enumerator should check the modification of cells in this row         /// and keep synchronized with it. |
**Returns**
The cells enumerator which will traverse all existing cells in this row.
**Remarks**
If the row will be modified(by operations that may cause new Cell be instantiated or existing Cell be removed) during the traversal with the enumerator, synchronized enumerator should be used instead of normal enumerator so that the traversal can continue from the position just after the one has been traversed by the last MoveNext(). However, together with the advantage that no element be skipped or traversed repeatedly, the disadvantage for synchronized enumerator is that the performance will be degraded a bit when comparing with normal enumerator.
### getCellOrNull(number) {#getCellOrNull-number-}
Gets the cell or null in the specific index.
```javascript
getCellOrNull(column: number) : Cell;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | The column index |
**Returns**
Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getStyle() {#getStyle--}
Gets the style of this row.
```javascript
getStyle() : Style;
```
**Returns**
[Style](../style/)
**Remarks**
Modifying the returned style object directly takes no effect for this row or any cells in this row. You have to call [ApplyStyle(Style, StyleFlag)](../applystyle(style, styleflag)/) or [SetStyle(Style)](../setstyle(style)/) method to apply the change to this row.<br></br> Row's style is the style which will be inherited by cells in this row(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)
### setStyle(Style) {#setStyle-style-}
Sets the style of this row.
```javascript
setStyle(style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | the style to be used as the default style for cells in this row. |
**Remarks**
This method only sets the given style as the default style for this row, without changing the style settings for existing cells in this row. To update style settings of existing cells to the specified style at the same time, please use [ApplyStyle(Style, StyleFlag)](../applystyle(style, styleflag)/)
### copySettings(Row, boolean) {#copySettings-row-boolean-}
Copy settings of row, such as style, height, visibility, ...etc.
```javascript
copySettings(source: Row, checkStyle: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Row](../row/) | the source row whose settings will be copied to this one |
| checkStyle | boolean | whether check and gather style.         /// Only takes effect and be needed when two row objects belong to different workbook and the styles of two workbooks are different. |
### applyStyle(Style, StyleFlag) {#applyStyle-style-styleflag-}
Applies formats for a whole row.
```javascript
applyStyle(style: Style, flag: StyleFlag) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The style object which will be applied. |
| flag | [StyleFlag](../styleflag/) | Flags which indicates applied formatting properties. |
### equals(VObject) {#equals-vobject-}
Checks whether this object refers to the same row with another.
```javascript
equals(obj: VObject) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | VObject | another object |
**Returns**
true if two objects refers to the same row.
### equals(Row) {#equals-row-}
Checks whether this object refers to the same row with another row object.
```javascript
equals(row: Row) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | [Row](../row/) | another row object |
**Returns**
true if two row objects refers to the same row.
