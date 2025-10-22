##TickLabels
Represents the tickmark labels associated with tick marks on a chart axis.
## TickLabels class
Represents the tick-mark labels associated with tick marks on a chart axis.
```javascript
class TickLabels;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [font](#font--)| Font | Readonly. Returns a [Font](../font/) object that represents the font of the specified TickLabels object. |
| [autoScaleFont](#autoScaleFont--)| boolean | True if the text in the object changes font size when the object size changes. The default value is True. |
| [backgroundMode](#backgroundMode--)| BackgroundMode | Gets and sets the display mode of the background |
| [rotationAngle](#rotationAngle--)| number | Represents text rotation angle in clockwise. |
| [isAutomaticRotation](#isAutomaticRotation--)| boolean | Indicates whether the rotation angle is automatic |
| [numberFormat](#numberFormat--)| string | Represents the format string for the TickLabels object. |
| [number](#number--)| number | Represents the format number for the TickLabels object. |
| [numberFormatLinked](#numberFormatLinked--)| boolean | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [displayNumberFormat](#displayNumberFormat--)| string | Readonly. Gets and sets the display number format of tick labels. |
| [offset](#offset--)| number | Gets and sets the distance of labels from the category axis. Only for category (x) axis. |
| [readingOrder](#readingOrder--)| TextDirectionType | Represents text reading order. |
| [directionType](#directionType--)| ChartTextDirectionType | Gets and sets the direction of text. |
| [tickLabelItems](#tickLabelItems--)| TickLabelItem[] | Readonly. Gets the display tick labels of the axis. |
| [alignmentType](#alignmentType--)| TickLabelAlignmentType | Gets and sets the text alignment for the tick labels on the axis. |
## Methods
| Method | Description |
| --- | --- |
| [getFont()](#getFont--)| <b>@deprecated.</b> Please use the 'font' property instead. Returns a [Font](../font/) object that represents the font of the specified TickLabels object. |
| [getAutoScaleFont()](#getAutoScaleFont--)| <b>@deprecated.</b> Please use the 'autoScaleFont' property instead. True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| <b>@deprecated.</b> Please use the 'autoScaleFont' property instead. True if the text in the object changes font size when the object size changes. The default value is True. |
| [getBackgroundMode()](#getBackgroundMode--)| <b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| <b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background |
| [getRotationAngle()](#getRotationAngle--)| <b>@deprecated.</b> Please use the 'rotationAngle' property instead. Represents text rotation angle in clockwise. |
| [setRotationAngle(number)](#setRotationAngle-number-)| <b>@deprecated.</b> Please use the 'rotationAngle' property instead. Represents text rotation angle in clockwise. |
| [isAutomaticRotation()](#isAutomaticRotation--)| <b>@deprecated.</b> Please use the 'isAutomaticRotation' property instead. Indicates whether the rotation angle is automatic |
| [setIsAutomaticRotation(boolean)](#setIsAutomaticRotation-boolean-)| <b>@deprecated.</b> Please use the 'isAutomaticRotation' property instead. Indicates whether the rotation angle is automatic |
| [get_NumberFormat()](#get_NumberFormat--)| <b>@deprecated.</b> Please use the 'numberFormat' property instead. Represents the format string for the TickLabels object. |
| [setNumberFormat(string)](#setNumberFormat-string-)| <b>@deprecated.</b> Please use the 'numberFormat' property instead. Represents the format string for the TickLabels object. |
| [getNumber()](#getNumber--)| <b>@deprecated.</b> Please use the 'number' property instead. Represents the format number for the TickLabels object. |
| [setNumber(number)](#setNumber-number-)| <b>@deprecated.</b> Please use the 'number' property instead. Represents the format number for the TickLabels object. |
| [getNumberFormatLinked()](#getNumberFormatLinked--)| <b>@deprecated.</b> Please use the 'numberFormatLinked' property instead. True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [setNumberFormatLinked(boolean)](#setNumberFormatLinked-boolean-)| <b>@deprecated.</b> Please use the 'numberFormatLinked' property instead. True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [getDisplayNumberFormat()](#getDisplayNumberFormat--)| <b>@deprecated.</b> Please use the 'displayNumberFormat' property instead. Gets and sets the display number format of tick labels. |
| [getOffset()](#getOffset--)| <b>@deprecated.</b> Please use the 'offset' property instead. Gets and sets the distance of labels from the category axis. Only for category (x) axis. |
| [setOffset(number)](#setOffset-number-)| <b>@deprecated.</b> Please use the 'offset' property instead. Gets and sets the distance of labels from the category axis. Only for category (x) axis. |
| [getReadingOrder()](#getReadingOrder--)| <b>@deprecated.</b> Please use the 'readingOrder' property instead. Represents text reading order. |
| [setReadingOrder(TextDirectionType)](#setReadingOrder-textdirectiontype-)| <b>@deprecated.</b> Please use the 'readingOrder' property instead. Represents text reading order. |
| [getDirectionType()](#getDirectionType--)| <b>@deprecated.</b> Please use the 'directionType' property instead. Gets and sets the direction of text. |
| [setDirectionType(ChartTextDirectionType)](#setDirectionType-charttextdirectiontype-)| <b>@deprecated.</b> Please use the 'directionType' property instead. Gets and sets the direction of text. |
| [getTickLabelItems()](#getTickLabelItems--)| <b>@deprecated.</b> Please use the 'tickLabelItems' property instead. Gets the display tick labels of the axis. |
| [getAlignmentType()](#getAlignmentType--)| <b>@deprecated.</b> Please use the 'alignmentType' property instead. Gets and sets the text alignment for the tick labels on the axis. |
| [setAlignmentType(TickLabelAlignmentType)](#setAlignmentType-ticklabelalignmenttype-)| <b>@deprecated.</b> Please use the 'alignmentType' property instead. Gets and sets the text alignment for the tick labels on the axis. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### font {#font--}
Readonly. Returns a [Font](../font/) object that represents the font of the specified TickLabels object.
```javascript
font : Font;
```
### autoScaleFont {#autoScaleFont--}
True if the text in the object changes font size when the object size changes. The default value is True.
```javascript
autoScaleFont : boolean;
```
### backgroundMode {#backgroundMode--}
Gets and sets the display mode of the background
```javascript
backgroundMode : BackgroundMode;
```
### rotationAngle {#rotationAngle--}
Represents text rotation angle in clockwise.
```javascript
rotationAngle : number;
```
**Remarks**
br>0: Not rotated.</br> <br>255: Top to Bottom.</br> <br>-90: Downward.</br> <br>90: Upward.</br
### isAutomaticRotation {#isAutomaticRotation--}
Indicates whether the rotation angle is automatic
```javascript
isAutomaticRotation : boolean;
```
### numberFormat {#numberFormat--}
Represents the format string for the TickLabels object.
```javascript
numberFormat : string;
```
**Remarks**
The formatting string is same as a custom format string setting to a cell. For example, "$0".
### number {#number--}
Represents the format number for the TickLabels object.
```javascript
number : number;
```
### numberFormatLinked {#numberFormatLinked--}
True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).
```javascript
numberFormatLinked : boolean;
```
### displayNumberFormat {#displayNumberFormat--}
Readonly. Gets and sets the display number format of tick labels.
```javascript
displayNumberFormat : string;
```
### offset {#offset--}
Gets and sets the distance of labels from the category axis. Only for category (x) axis.
```javascript
offset : number;
```
**Remarks**
The default distance is 100 percent, which represents the default spacing between the axis labels and the axis line. The value can be an integer percentage from 0 through 1000, relative to the axis label''s font size.
### readingOrder {#readingOrder--}
Represents text reading order.
```javascript
readingOrder : TextDirectionType;
```
### directionType {#directionType--}
Gets and sets the direction of text.
```javascript
directionType : ChartTextDirectionType;
```
### tickLabelItems {#tickLabelItems--}
Readonly. Gets the display tick labels of the axis.
```javascript
tickLabelItems : TickLabelItem[];
```
**Remarks**
Only available after calling [Chart.Calculate()](../chart.calculate()/) method.
### alignmentType {#alignmentType--}
Gets and sets the text alignment for the tick labels on the axis.
```javascript
alignmentType : TickLabelAlignmentType;
```
### getFont() {#getFont--}
```javascript
getFont() : Font;
```
**Returns**
[Font](../font/)
### getAutoScaleFont() {#getAutoScaleFont--}
```javascript
getAutoScaleFont() : boolean;
```
### setAutoScaleFont(boolean) {#setAutoScaleFont-boolean-}
```javascript
setAutoScaleFont(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getBackgroundMode() {#getBackgroundMode--}
```javascript
getBackgroundMode() : BackgroundMode;
```
**Returns**
[BackgroundMode](../backgroundmode/)
### setBackgroundMode(BackgroundMode) {#setBackgroundMode-backgroundmode-}
```javascript
setBackgroundMode(value: BackgroundMode) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BackgroundMode](../backgroundmode/) | The value to set. |
### getRotationAngle() {#getRotationAngle--}
```javascript
getRotationAngle() : number;
```
**Remarks**
br>0: Not rotated.</br> <br>255: Top to Bottom.</br> <br>-90: Downward.</br> <br>90: Upward.</br
### setRotationAngle(number) {#setRotationAngle-number-}
```javascript
setRotationAngle(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
br>0: Not rotated.</br> <br>255: Top to Bottom.</br> <br>-90: Downward.</br> <br>90: Upward.</br
### isAutomaticRotation() {#isAutomaticRotation--}
```javascript
isAutomaticRotation() : boolean;
```
### setIsAutomaticRotation(boolean) {#setIsAutomaticRotation-boolean-}
```javascript
setIsAutomaticRotation(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### get_NumberFormat() {#get_NumberFormat--}
```javascript
get_NumberFormat() : string;
```
**Remarks**
The formatting string is same as a custom format string setting to a cell. For example, "$0".
### setNumberFormat(string) {#setNumberFormat-string-}
```javascript
setNumberFormat(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
The formatting string is same as a custom format string setting to a cell. For example, "$0".
### getNumber() {#getNumber--}
```javascript
getNumber() : number;
```
### setNumber(number) {#setNumber-number-}
```javascript
setNumber(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getNumberFormatLinked() {#getNumberFormatLinked--}
```javascript
getNumberFormatLinked() : boolean;
```
### setNumberFormatLinked(boolean) {#setNumberFormatLinked-boolean-}
```javascript
setNumberFormatLinked(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDisplayNumberFormat() {#getDisplayNumberFormat--}
```javascript
getDisplayNumberFormat() : string;
```
### getOffset() {#getOffset--}
```javascript
getOffset() : number;
```
**Remarks**
The default distance is 100 percent, which represents the default spacing between the axis labels and the axis line. The value can be an integer percentage from 0 through 1000, relative to the axis label''s font size.
### setOffset(number) {#setOffset-number-}
```javascript
setOffset(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
The default distance is 100 percent, which represents the default spacing between the axis labels and the axis line. The value can be an integer percentage from 0 through 1000, relative to the axis label''s font size.
### getReadingOrder() {#getReadingOrder--}
```javascript
getReadingOrder() : TextDirectionType;
```
**Returns**
[TextDirectionType](../textdirectiontype/)
### setReadingOrder(TextDirectionType) {#setReadingOrder-textdirectiontype-}
```javascript
setReadingOrder(value: TextDirectionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextDirectionType](../textdirectiontype/) | The value to set. |
### getDirectionType() {#getDirectionType--}
```javascript
getDirectionType() : ChartTextDirectionType;
```
**Returns**
[ChartTextDirectionType](../charttextdirectiontype/)
### setDirectionType(ChartTextDirectionType) {#setDirectionType-charttextdirectiontype-}
```javascript
setDirectionType(value: ChartTextDirectionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartTextDirectionType](../charttextdirectiontype/) | The value to set. |
### getTickLabelItems() {#getTickLabelItems--}
```javascript
getTickLabelItems() : TickLabelItem[];
```
**Returns**
[TickLabelItem](../ticklabelitem/)[]
**Remarks**
Only available after calling [Chart.Calculate()](../chart.calculate()/) method.
### getAlignmentType() {#getAlignmentType--}
```javascript
getAlignmentType() : TickLabelAlignmentType;
```
**Returns**
[TickLabelAlignmentType](../ticklabelalignmenttype/)
### setAlignmentType(TickLabelAlignmentType) {#setAlignmentType-ticklabelalignmenttype-}
```javascript
setAlignmentType(value: TickLabelAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TickLabelAlignmentType](../ticklabelalignmenttype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
