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
