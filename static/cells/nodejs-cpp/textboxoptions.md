##TextBoxOptions
Represents the text options of the shape
## TextBoxOptions class
Represents the text options of the shape
```javascript
class TextBoxOptions;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [shapeTextVerticalAlignment](#shapeTextVerticalAlignment--)| ShapeTextVerticalAlignmentType | It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [resizeToFitText](#resizeToFitText--)| boolean | Indicates whether to resize the shape to fit the text |
| [shapeTextDirection](#shapeTextDirection--)| TextVerticalType | Gets or sets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel |
| [leftMarginPt](#leftMarginPt--)| number | Gets and sets the left margin in unit of Points. |
| [rightMarginPt](#rightMarginPt--)| number | Gets and sets the right margin in unit of Points. |
| [topMarginPt](#topMarginPt--)| number | Gets and sets the top margin in unit of Points. |
| [bottomMarginPt](#bottomMarginPt--)| number | Returns the bottom margin in unit of Points |
| [allowTextToOverflow](#allowTextToOverflow--)| boolean | Whether allow text to overflow shape. |
| [wrapTextInShape](#wrapTextInShape--)| boolean | Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body. |
## Methods
| Method | Description |
| --- | --- |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--)| <b>@deprecated.</b> Please use the 'shapeTextVerticalAlignment' property instead. It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType)](#setShapeTextVerticalAlignment-shapetextverticalalignmenttype-)| <b>@deprecated.</b> Please use the 'shapeTextVerticalAlignment' property instead. It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [getResizeToFitText()](#getResizeToFitText--)| <b>@deprecated.</b> Please use the 'resizeToFitText' property instead. Indicates whether to resize the shape to fit the text |
| [setResizeToFitText(boolean)](#setResizeToFitText-boolean-)| <b>@deprecated.</b> Please use the 'resizeToFitText' property instead. Indicates whether to resize the shape to fit the text |
| [getShapeTextDirection()](#getShapeTextDirection--)| <b>@deprecated.</b> Please use the 'shapeTextDirection' property instead. Gets or sets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel |
| [setShapeTextDirection(TextVerticalType)](#setShapeTextDirection-textverticaltype-)| <b>@deprecated.</b> Please use the 'shapeTextDirection' property instead. Gets or sets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel |
| [getLeftMarginPt()](#getLeftMarginPt--)| <b>@deprecated.</b> Please use the 'leftMarginPt' property instead. Gets and sets the left margin in unit of Points. |
| [setLeftMarginPt(number)](#setLeftMarginPt-number-)| <b>@deprecated.</b> Please use the 'leftMarginPt' property instead. Gets and sets the left margin in unit of Points. |
| [getRightMarginPt()](#getRightMarginPt--)| <b>@deprecated.</b> Please use the 'rightMarginPt' property instead. Gets and sets the right margin in unit of Points. |
| [setRightMarginPt(number)](#setRightMarginPt-number-)| <b>@deprecated.</b> Please use the 'rightMarginPt' property instead. Gets and sets the right margin in unit of Points. |
| [getTopMarginPt()](#getTopMarginPt--)| <b>@deprecated.</b> Please use the 'topMarginPt' property instead. Gets and sets the top margin in unit of Points. |
| [setTopMarginPt(number)](#setTopMarginPt-number-)| <b>@deprecated.</b> Please use the 'topMarginPt' property instead. Gets and sets the top margin in unit of Points. |
| [getBottomMarginPt()](#getBottomMarginPt--)| <b>@deprecated.</b> Please use the 'bottomMarginPt' property instead. Returns the bottom margin in unit of Points |
| [setBottomMarginPt(number)](#setBottomMarginPt-number-)| <b>@deprecated.</b> Please use the 'bottomMarginPt' property instead. Returns the bottom margin in unit of Points |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--)| <b>@deprecated.</b> Please use the 'allowTextToOverflow' property instead. Whether allow text to overflow shape. |
| [setAllowTextToOverflow(boolean)](#setAllowTextToOverflow-boolean-)| <b>@deprecated.</b> Please use the 'allowTextToOverflow' property instead. Whether allow text to overflow shape. |
| [getWrapTextInShape()](#getWrapTextInShape--)| <b>@deprecated.</b> Please use the 'wrapTextInShape' property instead. Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body. |
| [setWrapTextInShape(boolean)](#setWrapTextInShape-boolean-)| <b>@deprecated.</b> Please use the 'wrapTextInShape' property instead. Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### shapeTextVerticalAlignment {#shapeTextVerticalAlignment--}
It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.
```javascript
shapeTextVerticalAlignment : ShapeTextVerticalAlignmentType;
```
### resizeToFitText {#resizeToFitText--}
Indicates whether to resize the shape to fit the text
```javascript
resizeToFitText : boolean;
```
### shapeTextDirection {#shapeTextDirection--}
Gets or sets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel
```javascript
shapeTextDirection : TextVerticalType;
```
### leftMarginPt {#leftMarginPt--}
Gets and sets the left margin in unit of Points.
```javascript
leftMarginPt : number;
```
### rightMarginPt {#rightMarginPt--}
Gets and sets the right margin in unit of Points.
```javascript
rightMarginPt : number;
```
### topMarginPt {#topMarginPt--}
Gets and sets the top margin in unit of Points.
```javascript
topMarginPt : number;
```
### bottomMarginPt {#bottomMarginPt--}
Returns the bottom margin in unit of Points
```javascript
bottomMarginPt : number;
```
### allowTextToOverflow {#allowTextToOverflow--}
Whether allow text to overflow shape.
```javascript
allowTextToOverflow : boolean;
```
### wrapTextInShape {#wrapTextInShape--}
Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body.
```javascript
wrapTextInShape : boolean;
```
### getShapeTextVerticalAlignment() {#getShapeTextVerticalAlignment--}
```javascript
getShapeTextVerticalAlignment() : ShapeTextVerticalAlignmentType;
```
**Returns**
[ShapeTextVerticalAlignmentType](../shapetextverticalalignmenttype/)
### setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType) {#setShapeTextVerticalAlignment-shapetextverticalalignmenttype-}
```javascript
setShapeTextVerticalAlignment(value: ShapeTextVerticalAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ShapeTextVerticalAlignmentType](../shapetextverticalalignmenttype/) | The value to set. |
### getResizeToFitText() {#getResizeToFitText--}
```javascript
getResizeToFitText() : boolean;
```
### setResizeToFitText(boolean) {#setResizeToFitText-boolean-}
```javascript
setResizeToFitText(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShapeTextDirection() {#getShapeTextDirection--}
```javascript
getShapeTextDirection() : TextVerticalType;
```
**Returns**
[TextVerticalType](../textverticaltype/)
### setShapeTextDirection(TextVerticalType) {#setShapeTextDirection-textverticaltype-}
```javascript
setShapeTextDirection(value: TextVerticalType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextVerticalType](../textverticaltype/) | The value to set. |
### getLeftMarginPt() {#getLeftMarginPt--}
```javascript
getLeftMarginPt() : number;
```
### setLeftMarginPt(number) {#setLeftMarginPt-number-}
```javascript
setLeftMarginPt(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRightMarginPt() {#getRightMarginPt--}
```javascript
getRightMarginPt() : number;
```
### setRightMarginPt(number) {#setRightMarginPt-number-}
```javascript
setRightMarginPt(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getTopMarginPt() {#getTopMarginPt--}
```javascript
getTopMarginPt() : number;
```
### setTopMarginPt(number) {#setTopMarginPt-number-}
```javascript
setTopMarginPt(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBottomMarginPt() {#getBottomMarginPt--}
```javascript
getBottomMarginPt() : number;
```
### setBottomMarginPt(number) {#setBottomMarginPt-number-}
```javascript
setBottomMarginPt(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```javascript
getAllowTextToOverflow() : boolean;
```
### setAllowTextToOverflow(boolean) {#setAllowTextToOverflow-boolean-}
```javascript
setAllowTextToOverflow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getWrapTextInShape() {#getWrapTextInShape--}
```javascript
getWrapTextInShape() : boolean;
```
### setWrapTextInShape(boolean) {#setWrapTextInShape-boolean-}
```javascript
setWrapTextInShape(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
