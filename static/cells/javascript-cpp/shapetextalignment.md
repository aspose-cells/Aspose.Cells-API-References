##ShapeTextAlignment
Represents the setting of shapes text alignment
## ShapeTextAlignment class
Represents the setting of shape's text alignment;
```javascript
class ShapeTextAlignment;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isTextWrapped](#isTextWrapped--)| boolean | Gets or sets the text wrapped type of the shape which contains text. |
| [rotateTextWithShape](#rotateTextWithShape--)| boolean | Indicates whether rotating text with shape. |
| [textVerticalOverflow](#textVerticalOverflow--)| TextOverflowType | Gets and sets the text vertical overflow type of the text box. |
| [textHorizontalOverflow](#textHorizontalOverflow--)| TextOverflowType | Gets and sets the text horizontal overflow type of the text box. |
| [rotationAngle](#rotationAngle--)| number | Gets and sets the rotation of the shape. |
| [textVerticalType](#textVerticalType--)| TextVerticalType | Gets and sets the text direction. |
| [isLockedText](#isLockedText--)| boolean | Indicates whether the shape is locked when worksheet is protected. |
| [autoSize](#autoSize--)| boolean | Indicates if size of shape is adjusted automatically according to its content. |
| [textShapeType](#textShapeType--)| AutoShapeType | Gets and set the transform type of text. |
| [topMarginPt](#topMarginPt--)| number | Returns the top margin in unit of Points |
| [bottomMarginPt](#bottomMarginPt--)| number | Returns the bottom margin in unit of Points |
| [leftMarginPt](#leftMarginPt--)| number | Returns the left margin in unit of Points |
| [rightMarginPt](#rightMarginPt--)| number | Returns the right margin in unit of Points |
| [isAutoMargin](#isAutoMargin--)| boolean | Indicates whether the margin of the text frame is automatic. |
| [numberOfColumns](#numberOfColumns--)| number | Gets and sets the number of columns of text in the bounding rectangle. |
## Methods
| Method | Description |
| --- | --- |
| [equals(VObject)](#equals-vobject-)| Determines whether this instance has the same value as another specified [ShapeTextAlignment](../shapetextalignment/) object. |
| [getHashCode()](#getHashCode--)|  |
### isTextWrapped {#isTextWrapped--}
Gets or sets the text wrapped type of the shape which contains text.
```javascript
isTextWrapped : boolean;
```
### rotateTextWithShape {#rotateTextWithShape--}
Indicates whether rotating text with shape.
```javascript
rotateTextWithShape : boolean;
```
### textVerticalOverflow {#textVerticalOverflow--}
Gets and sets the text vertical overflow type of the text box.
```javascript
textVerticalOverflow : TextOverflowType;
```
### textHorizontalOverflow {#textHorizontalOverflow--}
Gets and sets the text horizontal overflow type of the text box.
```javascript
textHorizontalOverflow : TextOverflowType;
```
### rotationAngle {#rotationAngle--}
Gets and sets the rotation of the shape.
```javascript
rotationAngle : number;
```
### textVerticalType {#textVerticalType--}
Gets and sets the text direction.
```javascript
textVerticalType : TextVerticalType;
```
### isLockedText {#isLockedText--}
Indicates whether the shape is locked when worksheet is protected.
```javascript
isLockedText : boolean;
```
**Remarks**
Only works when worksheet is protected.
### autoSize {#autoSize--}
Indicates if size of shape is adjusted automatically according to its content.
```javascript
autoSize : boolean;
```
### textShapeType {#textShapeType--}
Gets and set the transform type of text.
```javascript
textShapeType : AutoShapeType;
```
### topMarginPt {#topMarginPt--}
Returns the top margin in unit of Points
```javascript
topMarginPt : number;
```
### bottomMarginPt {#bottomMarginPt--}
Returns the bottom margin in unit of Points
```javascript
bottomMarginPt : number;
```
### leftMarginPt {#leftMarginPt--}
Returns the left margin in unit of Points
```javascript
leftMarginPt : number;
```
### rightMarginPt {#rightMarginPt--}
Returns the right margin in unit of Points
```javascript
rightMarginPt : number;
```
### isAutoMargin {#isAutoMargin--}
Indicates whether the margin of the text frame is automatic.
```javascript
isAutoMargin : boolean;
```
### numberOfColumns {#numberOfColumns--}
Gets and sets the number of columns of text in the bounding rectangle.
```javascript
numberOfColumns : number;
```
### equals(VObject) {#equals-vobject-}
Determines whether this instance has the same value as another specified [ShapeTextAlignment](../shapetextalignment/) object.
```javascript
equals(obj: VObject) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | VObject | The [ShapeTextAlignment](../shapetextalignment/) object to compare with this instance. |
**Returns**
true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.
### getHashCode() {#getHashCode--}
```javascript
getHashCode() : number;
```
