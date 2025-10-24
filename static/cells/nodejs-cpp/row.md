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
| [isBlank()](#isBlank--)| <b>@deprecated.</b> Please use the 'isBlank' property instead. Indicates whether the row contains any data |
| [isCollapsed()](#isCollapsed--)| <b>@deprecated.</b> Please use the 'isCollapsed' property instead. whether the row is collapsed |
| [setIsCollapsed(boolean)](#setIsCollapsed-boolean-)| <b>@deprecated.</b> Please use the 'isCollapsed' property instead. whether the row is collapsed |
| [getHeight()](#getHeight--)| <b>@deprecated.</b> Please use the 'height' property instead. Gets and sets the row height in unit of Points. |
| [setHeight(number)](#setHeight-number-)| <b>@deprecated.</b> Please use the 'height' property instead. Gets and sets the row height in unit of Points. |
| [isHidden()](#isHidden--)| <b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether the row is hidden. |
| [setIsHidden(boolean)](#setIsHidden-boolean-)| <b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether the row is hidden. |
| [getIndex()](#getIndex--)| <b>@deprecated.</b> Please use the 'index' property instead. Gets the index of this row. |
| [getGroupLevel()](#getGroupLevel--)| <b>@deprecated.</b> Please use the 'groupLevel' property instead. Gets the group level of the row. |
| [setGroupLevel(number)](#setGroupLevel-number-)| <b>@deprecated.</b> Please use the 'groupLevel' property instead. Gets the group level of the row. |
| [isHeightMatched()](#isHeightMatched--)| <b>@deprecated.</b> Please use the 'isHeightMatched' property instead. Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user. |
| [setIsHeightMatched(boolean)](#setIsHeightMatched-boolean-)| <b>@deprecated.</b> Please use the 'isHeightMatched' property instead. Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user. |
| [getHasCustomStyle()](#getHasCustomStyle--)| <b>@deprecated.</b> Please use the 'hasCustomStyle' property instead. Indicates whether this row has custom style settings(different from the default one inherited from workbook). |
| [getFirstCell()](#getFirstCell--)| <b>@deprecated.</b> Please use the 'firstCell' property instead. Gets the first cell object in the row. |
| [getFirstDataCell()](#getFirstDataCell--)| <b>@deprecated.</b> Please use the 'firstDataCell' property instead. Gets the first non-blank cell in the row. |
| [getLastCell()](#getLastCell--)| <b>@deprecated.</b> Please use the 'lastCell' property instead. Gets the last cell object in the row. |
| [getLastDataCell()](#getLastDataCell--)| <b>@deprecated.</b> Please use the 'lastDataCell' property instead. Gets the last non-blank cell in the row. |
| [getCellByIndex(number)](#getCellByIndex-number-)| Get the cell by specific index in the cells collection of this row. |
| [getEnumerator()](#getEnumerator--)| Gets the cells enumerator |
| [getEnumerator(boolean, boolean)](#getEnumerator-boolean-boolean-)| Gets an enumerator that iterates cells through this row. |
| [getCellOrNull(number)](#getCellOrNull-number-)| Gets the cell or null in the specific index. |
| [getStyle()](#getStyle--)| Gets the style of this row. |
| [setStyle(Style)](#setStyle-style-)| Sets the style of this row. |
| [copySettings(Row, boolean)](#copySettings-row-boolean-)| Copy settings of row, such as style, height, visibility, ...etc. |
| [applyStyle(Style, StyleFlag)](#applyStyle-style-styleflag-)| Applies formats for a whole row. |
| [equals(Object)](#equals-object-)| Checks whether this object refers to the same row with another. |
| [equals(Row)](#equals-row-)| Checks whether this object refers to the same row with another row object. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### isBlank() {#isBlank--}
```javascript
isBlank() : boolean;
```
### isCollapsed() {#isCollapsed--}
```javascript
isCollapsed() : boolean;
```
### setIsCollapsed(boolean) {#setIsCollapsed-boolean-}
```javascript
setIsCollapsed(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getHeight() {#getHeight--}
```javascript
getHeight() : number;
```
### setHeight(number) {#setHeight-number-}
```javascript
setHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isHidden() {#isHidden--}
```javascript
isHidden() : boolean;
```
### setIsHidden(boolean) {#setIsHidden-boolean-}
```javascript
setIsHidden(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getIndex() {#getIndex--}
```javascript
getIndex() : number;
```
### getGroupLevel() {#getGroupLevel--}
```javascript
getGroupLevel() : number;
```
### setGroupLevel(number) {#setGroupLevel-number-}
```javascript
setGroupLevel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isHeightMatched() {#isHeightMatched--}
```javascript
isHeightMatched() : boolean;
```
**Remarks**
When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by [Worksheet.AutoFitRows()](../worksheet.autofitrows()/)) to get the same result with what is shown in ms excel when you opening the workbook in it.
### setIsHeightMatched(boolean) {#setIsHeightMatched-boolean-}
```javascript
setIsHeightMatched(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by [Worksheet.AutoFitRows()](../worksheet.autofitrows()/)) to get the same result with what is shown in ms excel when you opening the workbook in it.
### getHasCustomStyle() {#getHasCustomStyle--}
```javascript
getHasCustomStyle() : boolean;
```
### getFirstCell() {#getFirstCell--}
```javascript
getFirstCell() : Cell;
```
**Returns**
[Cell](../cell/)
### getFirstDataCell() {#getFirstDataCell--}
```javascript
getFirstDataCell() : Cell;
```
**Returns**
[Cell](../cell/)
### getLastCell() {#getLastCell--}
```javascript
getLastCell() : Cell;
```
**Returns**
[Cell](../cell/)
### getLastDataCell() {#getLastDataCell--}
```javascript
getLastDataCell() : Cell;
```
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
### equals(Object) {#equals-object-}
Checks whether this object refers to the same row with another.
```javascript
equals(obj: Object) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | another object |
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
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
