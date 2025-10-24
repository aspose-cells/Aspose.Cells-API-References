##DataBar
Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells.
## DataBar class
Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells.
```javascript
class DataBar;
```
### Example
```javascript
const { Workbook, CellArea, Color, FormatConditionType, FormatConditionValueType } = require("aspose.cells.node");
//Instantiating a Workbook object
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);
//Adds an empty conditional formatting
var index = sheet.conditionalFormattings.add();
var fcs = sheet.conditionalFormattings.get(index);
//Sets the conditional format range.
var ca = new CellArea();
ca.startRow = 0;
ca.endRow = 2;
ca.startColumn = 0;
ca.endColumn = 0;
fcs.addArea(ca);
//Adds condition.
var idx = fcs.addCondition(FormatConditionType.DataBar);
fcs.addArea(ca);
var cond = fcs.get(idx);
//Get Databar
var dataBar = cond.dataBar;
var orange = Color.Orange;
dataBar.color = orange;
//Set Databar properties
dataBar.minCfvo.type = FormatConditionValueType.Percentile;
dataBar.minCfvo.value = 30;
dataBar.showValue = false;
//Put Cell Values
var cell1 = sheet.cells.get("A1");
cell1.putValue(10);
var cell2 = sheet.cells.get("A2");
cell2.putValue(120);
var cell3 = sheet.cells.get("A3");
cell3.putValue(260);
//Saving the Excel file
workbook.save("output/DataBar.xlsx");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [axisColor](#axisColor--)| Color | Gets the color of the axis for cells with conditional formatting as data bars. |
| [axisPosition](#axisPosition--)| DataBarAxisPosition | Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [barFillType](#barFillType--)| DataBarFillType | Gets or sets how a data bar is filled with color. |
| [direction](#direction--)| TextDirectionType | Gets or sets the direction the databar is displayed. |
| [barBorder](#barBorder--)| DataBarBorder | Readonly. Gets an object that specifies the border of a data bar. |
| [negativeBarFormat](#negativeBarFormat--)| NegativeBarFormat | Readonly. Gets the NegativeBarFormat object associated with a data bar conditional formatting rule. |
| [minCfvo](#minCfvo--)| ConditionalFormattingValue | Readonly. Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
| [maxCfvo](#maxCfvo--)| ConditionalFormattingValue | Readonly. Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
| [color](#color--)| Color | Get or set this DataBar's Color. |
| [minLength](#minLength--)| number | Represents the min length of data bar . |
| [maxLength](#maxLength--)| number | Represents the max length of data bar . |
| [showValue](#showValue--)| boolean | Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true. |
## Methods
| Method | Description |
| --- | --- |
| [getAxisColor()](#getAxisColor--)| <b>@deprecated.</b> Please use the 'axisColor' property instead. Gets the color of the axis for cells with conditional formatting as data bars. |
| [setAxisColor(Color)](#setAxisColor-color-)| <b>@deprecated.</b> Please use the 'axisColor' property instead. Gets the color of the axis for cells with conditional formatting as data bars. |
| [getAxisPosition()](#getAxisPosition--)| <b>@deprecated.</b> Please use the 'axisPosition' property instead. Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [setAxisPosition(DataBarAxisPosition)](#setAxisPosition-databaraxisposition-)| <b>@deprecated.</b> Please use the 'axisPosition' property instead. Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [getBarFillType()](#getBarFillType--)| <b>@deprecated.</b> Please use the 'barFillType' property instead. Gets or sets how a data bar is filled with color. |
| [setBarFillType(DataBarFillType)](#setBarFillType-databarfilltype-)| <b>@deprecated.</b> Please use the 'barFillType' property instead. Gets or sets how a data bar is filled with color. |
| [getDirection()](#getDirection--)| <b>@deprecated.</b> Please use the 'direction' property instead. Gets or sets the direction the databar is displayed. |
| [setDirection(TextDirectionType)](#setDirection-textdirectiontype-)| <b>@deprecated.</b> Please use the 'direction' property instead. Gets or sets the direction the databar is displayed. |
| [getBarBorder()](#getBarBorder--)| <b>@deprecated.</b> Please use the 'barBorder' property instead. Gets an object that specifies the border of a data bar. |
| [getNegativeBarFormat()](#getNegativeBarFormat--)| <b>@deprecated.</b> Please use the 'negativeBarFormat' property instead. Gets the NegativeBarFormat object associated with a data bar conditional formatting rule. |
| [getMinCfvo()](#getMinCfvo--)| <b>@deprecated.</b> Please use the 'minCfvo' property instead. Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
| [getMaxCfvo()](#getMaxCfvo--)| <b>@deprecated.</b> Please use the 'maxCfvo' property instead. Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Get or set this DataBar's Color. |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Get or set this DataBar's Color. |
| [getMinLength()](#getMinLength--)| <b>@deprecated.</b> Please use the 'minLength' property instead. Represents the min length of data bar . |
| [setMinLength(number)](#setMinLength-number-)| <b>@deprecated.</b> Please use the 'minLength' property instead. Represents the min length of data bar . |
| [getMaxLength()](#getMaxLength--)| <b>@deprecated.</b> Please use the 'maxLength' property instead. Represents the max length of data bar . |
| [setMaxLength(number)](#setMaxLength-number-)| <b>@deprecated.</b> Please use the 'maxLength' property instead. Represents the max length of data bar . |
| [getShowValue()](#getShowValue--)| <b>@deprecated.</b> Please use the 'showValue' property instead. Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true. |
| [setShowValue(boolean)](#setShowValue-boolean-)| <b>@deprecated.</b> Please use the 'showValue' property instead. Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true. |
| [toImage(Cell, ImageOrPrintOptions)](#toImage-cell-imageorprintoptions-)| Render data bar in cell to image byte array. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### axisColor {#axisColor--}
Gets the color of the axis for cells with conditional formatting as data bars.
```javascript
axisColor : Color;
```
### axisPosition {#axisPosition--}
Gets or sets the position of the axis of the data bars specified by a conditional formatting rule.
```javascript
axisPosition : DataBarAxisPosition;
```
### barFillType {#barFillType--}
Gets or sets how a data bar is filled with color.
```javascript
barFillType : DataBarFillType;
```
### direction {#direction--}
Gets or sets the direction the databar is displayed.
```javascript
direction : TextDirectionType;
```
### barBorder {#barBorder--}
Readonly. Gets an object that specifies the border of a data bar.
```javascript
barBorder : DataBarBorder;
```
### negativeBarFormat {#negativeBarFormat--}
Readonly. Gets the NegativeBarFormat object associated with a data bar conditional formatting rule.
```javascript
negativeBarFormat : NegativeBarFormat;
```
### minCfvo {#minCfvo--}
Readonly. Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.
```javascript
minCfvo : ConditionalFormattingValue;
```
### maxCfvo {#maxCfvo--}
Readonly. Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it.
```javascript
maxCfvo : ConditionalFormattingValue;
```
### color {#color--}
Get or set this DataBar's Color.
```javascript
color : Color;
```
### minLength {#minLength--}
Represents the min length of data bar .
```javascript
minLength : number;
```
### maxLength {#maxLength--}
Represents the max length of data bar .
```javascript
maxLength : number;
```
### showValue {#showValue--}
Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true.
```javascript
showValue : boolean;
```
### getAxisColor() {#getAxisColor--}
```javascript
getAxisColor() : Color;
```
**Returns**
[Color](../color/)
### setAxisColor(Color) {#setAxisColor-color-}
```javascript
setAxisColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getAxisPosition() {#getAxisPosition--}
```javascript
getAxisPosition() : DataBarAxisPosition;
```
**Returns**
[DataBarAxisPosition](../databaraxisposition/)
### setAxisPosition(DataBarAxisPosition) {#setAxisPosition-databaraxisposition-}
```javascript
setAxisPosition(value: DataBarAxisPosition) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DataBarAxisPosition](../databaraxisposition/) | The value to set. |
### getBarFillType() {#getBarFillType--}
```javascript
getBarFillType() : DataBarFillType;
```
**Returns**
[DataBarFillType](../databarfilltype/)
### setBarFillType(DataBarFillType) {#setBarFillType-databarfilltype-}
```javascript
setBarFillType(value: DataBarFillType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DataBarFillType](../databarfilltype/) | The value to set. |
### getDirection() {#getDirection--}
```javascript
getDirection() : TextDirectionType;
```
**Returns**
[TextDirectionType](../textdirectiontype/)
### setDirection(TextDirectionType) {#setDirection-textdirectiontype-}
```javascript
setDirection(value: TextDirectionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextDirectionType](../textdirectiontype/) | The value to set. |
### getBarBorder() {#getBarBorder--}
```javascript
getBarBorder() : DataBarBorder;
```
**Returns**
[DataBarBorder](../databarborder/)
### getNegativeBarFormat() {#getNegativeBarFormat--}
```javascript
getNegativeBarFormat() : NegativeBarFormat;
```
**Returns**
[NegativeBarFormat](../negativebarformat/)
### getMinCfvo() {#getMinCfvo--}
```javascript
getMinCfvo() : ConditionalFormattingValue;
```
**Returns**
[ConditionalFormattingValue](../conditionalformattingvalue/)
### getMaxCfvo() {#getMaxCfvo--}
```javascript
getMaxCfvo() : ConditionalFormattingValue;
```
**Returns**
[ConditionalFormattingValue](../conditionalformattingvalue/)
### getColor() {#getColor--}
```javascript
getColor() : Color;
```
**Returns**
[Color](../color/)
### setColor(Color) {#setColor-color-}
```javascript
setColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getMinLength() {#getMinLength--}
```javascript
getMinLength() : number;
```
### setMinLength(number) {#setMinLength-number-}
```javascript
setMinLength(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getMaxLength() {#getMaxLength--}
```javascript
getMaxLength() : number;
```
### setMaxLength(number) {#setMaxLength-number-}
```javascript
setMaxLength(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getShowValue() {#getShowValue--}
```javascript
getShowValue() : boolean;
```
### setShowValue(boolean) {#setShowValue-boolean-}
```javascript
setShowValue(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### toImage(Cell, ImageOrPrintOptions) {#toImage-cell-imageorprintoptions-}
Render data bar in cell to image byte array.
```javascript
toImage(cell: Cell, imgOpts: ImageOrPrintOptions) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../cell/) | Indicate the data bar in which cell to be rendered |
| imgOpts | [ImageOrPrintOptions](../imageorprintoptions/) | ImageOrPrintOptions contains some property of output image |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
