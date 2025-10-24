##DisplayUnitLabel
Represents the display unit label.
## DisplayUnitLabel class
Represents the display unit label.
```javascript
class DisplayUnitLabel extends ChartTextFrame;
```
### Example
```javascript
const { Workbook, ChartType, DisplayUnitType } = require("aspose.cells.node");
//Instantiating a Workbook object
var workbook = new Workbook();
//Adding a new worksheet to the Excel object
var sheetIndex = workbook.worksheets.add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.cells.get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.cells.get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.cells.get("A3").putValue(150);
//Adding a sample value to "A4" cell
worksheet.cells.get("A4").putValue(200);
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);
//Adding a sample value to "B4" cell
worksheet.cells.get("B4").putValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").putValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").putValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").putValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").putValue("Y2");
//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.nSeries.add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.nSeries.categoryData = "C1:C4";
//Setting the display unit of value(Y) axis.
chart.valueAxis.sisplayUnit = DisplayUnitType.Hundreds;
var displayUnitLabel = chart.valueAxis.displayUnitLabel;
//Setting the custom display unit label
displayUnitLabel.text = "100";
//Saving the Excel file
workbook.save("output/ChartsDisplayUnitLabel.xls");
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(ChartTextFrame)](#constructor-charttextframe-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isInnerMode](#isInnerMode--)| boolean | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [backgroundMode](#backgroundMode--)| BackgroundMode | Gets and sets the display mode of the background |
| [shadow](#shadow--)| boolean | True if the frame has a shadow. |
| [shapeProperties](#shapeProperties--)| ShapePropertyCollection | Readonly. Gets the [ShapeProperties](../shapeproperties/) object. |
| [isDefaultPosBeSet](#isDefaultPosBeSet--)| boolean | Readonly. Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [defaultX](#defaultX--)| number | Readonly. Represents x of default position in units of 1/4000 of the chart area. |
| [defaultY](#defaultY--)| number | Readonly. Represents y of default position in units of 1/4000 of the chart area. |
| [defaultWidth](#defaultWidth--)| number | Readonly. Represents width of default position in units of 1/4000 of the chart area. |
| [defaultHeight](#defaultHeight--)| number | Readonly. Represents height of default position in units of 1/4000 of the chart area. |
| [defaultXRatioToChart](#defaultXRatioToChart--)| number | Readonly. Represents x of default position in units of Fraction of the chart area. |
| [defaultYRatioToChart](#defaultYRatioToChart--)| number | Readonly. Represents y of default position in units of Fraction of the chart area. |
| [defaultWidthRatioToChart](#defaultWidthRatioToChart--)| number | Readonly. Represents width of default position in units of Fraction of the chart area. |
| [defaultHeightRatioToChart](#defaultHeightRatioToChart--)| number | Readonly. Represents height of default position in units of Fraction of the chart area. |
| [isDeleted](#isDeleted--)| boolean | Indicates whether this data labels is deleted. |
| [textHorizontalAlignment](#textHorizontalAlignment--)| TextAlignmentType | Gets and sets the text horizontal alignment. |
| [textVerticalAlignment](#textVerticalAlignment--)| TextAlignmentType | Gets or sets the text vertical alignment of text. |
| [rotationAngle](#rotationAngle--)| number | Represents text rotation angle. |
| [isAutomaticRotation](#isAutomaticRotation--)| boolean | Readonly. Indicates whether the text of the chart is automatically rotated. |
| [readingOrder](#readingOrder--)| TextDirectionType | Represents text reading order. |
| [isResizeShapeToFitText](#isResizeShapeToFitText--)| boolean | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [isInnerMode()](#isInnerMode--)| <b>@deprecated.</b> Please use the 'isInnerMode' property instead. Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [setIsInnerMode(boolean)](#setIsInnerMode-boolean-)| <b>@deprecated.</b> Please use the 'isInnerMode' property instead. Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [getBackgroundMode()](#getBackgroundMode--)| <b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| <b>@deprecated.</b> Please use the 'backgroundMode' property instead. Gets and sets the display mode of the background |
| [getShadow()](#getShadow--)| <b>@deprecated.</b> Please use the 'shadow' property instead. True if the frame has a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| <b>@deprecated.</b> Please use the 'shadow' property instead. True if the frame has a shadow. |
| [getShapeProperties()](#getShapeProperties--)| <b>@deprecated.</b> Please use the 'shapeProperties' property instead. Gets the [ShapeProperties](../shapeproperties/) object. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--)| <b>@deprecated.</b> Please use the 'isDefaultPosBeSet' property instead. Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [getDefaultX()](#getDefaultX--)| <b>@deprecated.</b> Please use the 'defaultX' property instead. Represents x of default position in units of 1/4000 of the chart area. |
| [getDefaultY()](#getDefaultY--)| <b>@deprecated.</b> Please use the 'defaultY' property instead. Represents y of default position in units of 1/4000 of the chart area. |
| [getDefaultWidth()](#getDefaultWidth--)| <b>@deprecated.</b> Please use the 'defaultWidth' property instead. Represents width of default position in units of 1/4000 of the chart area. |
| [getDefaultHeight()](#getDefaultHeight--)| <b>@deprecated.</b> Please use the 'defaultHeight' property instead. Represents height of default position in units of 1/4000 of the chart area. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--)| <b>@deprecated.</b> Please use the 'defaultXRatioToChart' property instead. Represents x of default position in units of Fraction of the chart area. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--)| <b>@deprecated.</b> Please use the 'defaultYRatioToChart' property instead. Represents y of default position in units of Fraction of the chart area. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--)| <b>@deprecated.</b> Please use the 'defaultWidthRatioToChart' property instead. Represents width of default position in units of Fraction of the chart area. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--)| <b>@deprecated.</b> Please use the 'defaultHeightRatioToChart' property instead. Represents height of default position in units of Fraction of the chart area. |
| [isDeleted()](#isDeleted--)| <b>@deprecated.</b> Please use the 'isDeleted' property instead. Indicates whether this data labels is deleted. |
| [setIsDeleted(boolean)](#setIsDeleted-boolean-)| <b>@deprecated.</b> Please use the 'isDeleted' property instead. Indicates whether this data labels is deleted. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--)| <b>@deprecated.</b> Please use the 'textHorizontalAlignment' property instead. Gets and sets the text horizontal alignment. |
| [setTextHorizontalAlignment(TextAlignmentType)](#setTextHorizontalAlignment-textalignmenttype-)| <b>@deprecated.</b> Please use the 'textHorizontalAlignment' property instead. Gets and sets the text horizontal alignment. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--)| <b>@deprecated.</b> Please use the 'textVerticalAlignment' property instead. Gets or sets the text vertical alignment of text. |
| [setTextVerticalAlignment(TextAlignmentType)](#setTextVerticalAlignment-textalignmenttype-)| <b>@deprecated.</b> Please use the 'textVerticalAlignment' property instead. Gets or sets the text vertical alignment of text. |
| [getRotationAngle()](#getRotationAngle--)| <b>@deprecated.</b> Please use the 'rotationAngle' property instead. Represents text rotation angle. |
| [setRotationAngle(number)](#setRotationAngle-number-)| <b>@deprecated.</b> Please use the 'rotationAngle' property instead. Represents text rotation angle. |
| [isAutomaticRotation()](#isAutomaticRotation--)| <b>@deprecated.</b> Please use the 'isAutomaticRotation' property instead. Indicates whether the text of the chart is automatically rotated. |
| [getReadingOrder()](#getReadingOrder--)| <b>@deprecated.</b> Please use the 'readingOrder' property instead. Represents text reading order. |
| [setReadingOrder(TextDirectionType)](#setReadingOrder-textdirectiontype-)| <b>@deprecated.</b> Please use the 'readingOrder' property instead. Represents text reading order. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--)| <b>@deprecated.</b> Please use the 'isResizeShapeToFitText' property instead. Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [setIsResizeShapeToFitText(boolean)](#setIsResizeShapeToFitText-boolean-)| <b>@deprecated.</b> Please use the 'isResizeShapeToFitText' property instead. Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the text. |
| [getText()](#getText--)| Gets or sets the text of display unit label. |
| [setText(string)](#setText-string-)| Gets or sets the text of display unit label. |
| [getFont()](#getFont--)| Gets a [Font](../font/) object of the specified ChartFrame object. |
| [getAutoScaleFont()](#getAutoScaleFont--)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [getBorder()](#getBorder--)| Gets the <see cref="Line">border</see>. |
| [getArea()](#getArea--)| Gets the <see cref="Area">area</see>. |
| [getTextOptions()](#getTextOptions--)| Gets and sets the options of the text. |
| [isAutomaticSize()](#isAutomaticSize--)| Indicates whether the chart frame is automatic sized. |
| [setIsAutomaticSize(boolean)](#setIsAutomaticSize-boolean-)| Indicates whether the chart frame is automatic sized. |
| [getX()](#getX--)| Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [setX(number)](#setX-number-)| Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [getY()](#getY--)| Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [setY(number)](#setY-number-)| Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [getHeight()](#getHeight--)| Gets or sets the height of frame in units of 1/4000 of the chart area. |
| [setHeight(number)](#setHeight-number-)| Gets or sets the height of frame in units of 1/4000 of the chart area. |
| [getWidth()](#getWidth--)| Gets or sets the width of frame in units of 1/4000 of the chart area. |
| [setWidth(number)](#setWidth-number-)| Gets or sets the width of frame in units of 1/4000 of the chart area. |
| [getXRatioToChart()](#getXRatioToChart--)| Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area. |
| [setXRatioToChart(number)](#setXRatioToChart-number-)| Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area. |
| [getYRatioToChart()](#getYRatioToChart--)| Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area. |
| [setYRatioToChart(number)](#setYRatioToChart-number-)| Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area. |
| [getWidthRatioToChart()](#getWidthRatioToChart--)| Gets or sets the width of frame in units of ratio of the chart area. |
| [setWidthRatioToChart(number)](#setWidthRatioToChart-number-)| Gets or sets the width of frame in units of ratio of the chart area. |
| [getHeightRatioToChart()](#getHeightRatioToChart--)| Gets or sets the height of frame in units of ratio of the chart area. |
| [setHeightRatioToChart(number)](#setHeightRatioToChart-number-)| Gets or sets the height of frame in units of ratio of the chart area. |
| [getXPixel()](#getXPixel--)| Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [setXPixel(number)](#setXPixel-number-)| Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [getYPixel()](#getYPixel--)| Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [setYPixel(number)](#setYPixel-number-)| Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [getWidthPixel()](#getWidthPixel--)| Gets or sets the width of frame in units of Pixel. |
| [setWidthPixel(number)](#setWidthPixel-number-)| Gets or sets the width of frame in units of Pixel. |
| [getHeightPixel()](#getHeightPixel--)| Gets or sets the height of frame in units of Pixel. |
| [setHeightPixel(number)](#setHeightPixel-number-)| Gets or sets the height of frame in units of Pixel. |
| [setPositionAuto()](#setPositionAuto--)| Set position of the frame to automatic |
| [isAutoText()](#isAutoText--)| Indicates the text is auto generated. |
| [setIsAutoText(boolean)](#setIsAutoText-boolean-)| Indicates the text is auto generated. |
| [getLinkedSource()](#getLinkedSource--)| Gets and sets a reference to the worksheet. |
| [setLinkedSource(string)](#setLinkedSource-string-)| Gets and sets a reference to the worksheet. |
| [getDirectionType()](#getDirectionType--)| Gets and sets the direction of text. |
| [setDirectionType(ChartTextDirectionType)](#setDirectionType-charttextdirectiontype-)| Gets and sets the direction of text. |
| [isTextWrapped()](#isTextWrapped--)| Gets or sets a value indicating whether the text is wrapped. |
| [setIsTextWrapped(boolean)](#setIsTextWrapped-boolean-)| Gets or sets a value indicating whether the text is wrapped. |
### constructor(ChartTextFrame) {#constructor-charttextframe-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: ChartTextFrame);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ChartTextFrame | The parent object. |
### isInnerMode {#isInnerMode--}
Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.
```javascript
isInnerMode : boolean;
```
**Remarks**
Only for Xlsx file.
### backgroundMode {#backgroundMode--}
Gets and sets the display mode of the background
```javascript
backgroundMode : BackgroundMode;
```
### shadow {#shadow--}
True if the frame has a shadow.
```javascript
shadow : boolean;
```
### shapeProperties {#shapeProperties--}
Readonly. Gets the [ShapeProperties](../shapeproperties/) object.
```javascript
shapeProperties : ShapePropertyCollection;
```
### isDefaultPosBeSet {#isDefaultPosBeSet--}
Readonly. Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.
```javascript
isDefaultPosBeSet : boolean;
```
### defaultX {#defaultX--}
Readonly. Represents x of default position in units of 1/4000 of the chart area.
```javascript
defaultX : number;
```
**Remarks**
NOTE: This member is now obsolete. Please use ChartFrame.DefaultXRatioToChart property, instead. DefaultX = (int)(DefaultXRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### defaultY {#defaultY--}
Readonly. Represents y of default position in units of 1/4000 of the chart area.
```javascript
defaultY : number;
```
**Remarks**
NOTE: This member is now obsolete. Please use ChartFrame.DefaultYRatioToChart property, instead. DefaultY = (int)(DefaultYRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### defaultWidth {#defaultWidth--}
Readonly. Represents width of default position in units of 1/4000 of the chart area.
```javascript
defaultWidth : number;
```
**Remarks**
NOTE: This member is now obsolete. Please use ChartFrame.DefaultWidthRatioToChart property, instead. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### defaultHeight {#defaultHeight--}
Readonly. Represents height of default position in units of 1/4000 of the chart area.
```javascript
defaultHeight : number;
```
**Remarks**
NOTE: This member is now obsolete. Please use ChartFrame.DefaultHeightRatioToChart property, instead. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### defaultXRatioToChart {#defaultXRatioToChart--}
Readonly. Represents x of default position in units of Fraction of the chart area.
```javascript
defaultXRatioToChart : number;
```
### defaultYRatioToChart {#defaultYRatioToChart--}
Readonly. Represents y of default position in units of Fraction of the chart area.
```javascript
defaultYRatioToChart : number;
```
### defaultWidthRatioToChart {#defaultWidthRatioToChart--}
Readonly. Represents width of default position in units of Fraction of the chart area.
```javascript
defaultWidthRatioToChart : number;
```
### defaultHeightRatioToChart {#defaultHeightRatioToChart--}
Readonly. Represents height of default position in units of Fraction of the chart area.
```javascript
defaultHeightRatioToChart : number;
```
### isDeleted {#isDeleted--}
Indicates whether this data labels is deleted.
```javascript
isDeleted : boolean;
```
### textHorizontalAlignment {#textHorizontalAlignment--}
Gets and sets the text horizontal alignment.
```javascript
textHorizontalAlignment : TextAlignmentType;
```
### textVerticalAlignment {#textVerticalAlignment--}
Gets or sets the text vertical alignment of text.
```javascript
textVerticalAlignment : TextAlignmentType;
```
### rotationAngle {#rotationAngle--}
Represents text rotation angle.
```javascript
rotationAngle : number;
```
**Remarks**
br>0: Not rotated.</br> <br>255: Top to Bottom.</br> <br>-90: Downward.</br> <br>90: Upward.</br
### isAutomaticRotation {#isAutomaticRotation--}
Readonly. Indicates whether the text of the chart is automatically rotated.
```javascript
isAutomaticRotation : boolean;
```
### readingOrder {#readingOrder--}
Represents text reading order.
```javascript
readingOrder : TextDirectionType;
```
### isResizeShapeToFitText {#isResizeShapeToFitText--}
Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.
```javascript
isResizeShapeToFitText : boolean;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### isInnerMode() {#isInnerMode--}
```javascript
isInnerMode() : boolean;
```
**Remarks**
Only for Xlsx file.
### setIsInnerMode(boolean) {#setIsInnerMode-boolean-}
```javascript
setIsInnerMode(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only for Xlsx file.
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
### getShadow() {#getShadow--}
```javascript
getShadow() : boolean;
```
### setShadow(boolean) {#setShadow-boolean-}
```javascript
setShadow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShapeProperties() {#getShapeProperties--}
```javascript
getShapeProperties() : ShapePropertyCollection;
```
**Returns**
[ShapePropertyCollection](../shapepropertycollection/)
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```javascript
isDefaultPosBeSet() : boolean;
```
### getDefaultX() {#getDefaultX--}
```javascript
getDefaultX() : number;
```
**Remarks**
NOTE: This member is now obsolete. Please use ChartFrame.DefaultXRatioToChart property, instead. DefaultX = (int)(DefaultXRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### getDefaultY() {#getDefaultY--}
```javascript
getDefaultY() : number;
```
**Remarks**
NOTE: This member is now obsolete. Please use ChartFrame.DefaultYRatioToChart property, instead. DefaultY = (int)(DefaultYRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### getDefaultWidth() {#getDefaultWidth--}
```javascript
getDefaultWidth() : number;
```
**Remarks**
NOTE: This member is now obsolete. Please use ChartFrame.DefaultWidthRatioToChart property, instead. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### getDefaultHeight() {#getDefaultHeight--}
```javascript
getDefaultHeight() : number;
```
**Remarks**
NOTE: This member is now obsolete. Please use ChartFrame.DefaultHeightRatioToChart property, instead. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```javascript
getDefaultXRatioToChart() : number;
```
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```javascript
getDefaultYRatioToChart() : number;
```
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```javascript
getDefaultWidthRatioToChart() : number;
```
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```javascript
getDefaultHeightRatioToChart() : number;
```
### isDeleted() {#isDeleted--}
```javascript
isDeleted() : boolean;
```
### setIsDeleted(boolean) {#setIsDeleted-boolean-}
```javascript
setIsDeleted(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```javascript
getTextHorizontalAlignment() : TextAlignmentType;
```
**Returns**
[TextAlignmentType](../textalignmenttype/)
### setTextHorizontalAlignment(TextAlignmentType) {#setTextHorizontalAlignment-textalignmenttype-}
```javascript
setTextHorizontalAlignment(value: TextAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```javascript
getTextVerticalAlignment() : TextAlignmentType;
```
**Returns**
[TextAlignmentType](../textalignmenttype/)
### setTextVerticalAlignment(TextAlignmentType) {#setTextVerticalAlignment-textalignmenttype-}
```javascript
setTextVerticalAlignment(value: TextAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |
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
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```javascript
isResizeShapeToFitText() : boolean;
```
### setIsResizeShapeToFitText(boolean) {#setIsResizeShapeToFitText-boolean-}
```javascript
setIsResizeShapeToFitText(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### characters(number, number) {#characters-number-number-}
Returns a Characters object that represents a range of characters within the text.
```javascript
characters(startIndex: number, length: number) : FontSetting;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The index of the start of the character. |
| length | number | The number of characters. |
**Returns**
Characters object.
### getText() {#getText--}
Gets or sets the text of display unit label.
```javascript
getText() : string;
```
### setText(string) {#setText-string-}
Gets or sets the text of display unit label.
```javascript
setText(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getFont() {#getFont--}
Gets a [Font](../font/) object of the specified ChartFrame object.
```javascript
getFont() : Font;
```
**Returns**
[Font](../font/)
### getAutoScaleFont() {#getAutoScaleFont--}
True if the text in the object changes font size when the object size changes. The default value is True.
```javascript
getAutoScaleFont() : boolean;
```
### setAutoScaleFont(boolean) {#setAutoScaleFont-boolean-}
True if the text in the object changes font size when the object size changes. The default value is True.
```javascript
setAutoScaleFont(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getBorder() {#getBorder--}
Gets the <see cref="Line">border</see>.
```javascript
getBorder() : Line;
```
**Returns**
[Line](../line/)
### getArea() {#getArea--}
Gets the <see cref="Area">area</see>.
```javascript
getArea() : Area;
```
**Returns**
[Area](../area/)
### getTextOptions() {#getTextOptions--}
Gets and sets the options of the text.
```javascript
getTextOptions() : TextOptions;
```
**Returns**
[TextOptions](../textoptions/)
### isAutomaticSize() {#isAutomaticSize--}
Indicates whether the chart frame is automatic sized.
```javascript
isAutomaticSize() : boolean;
```
### setIsAutomaticSize(boolean) {#setIsAutomaticSize-boolean-}
Indicates whether the chart frame is automatic sized.
```javascript
setIsAutomaticSize(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getX() {#getX--}
Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.
```javascript
getX() : number;
```
**Remarks**
How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000d;
### setX(number) {#setX-number-}
Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.
```javascript
setX(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000d;
### getY() {#getY--}
Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.
```javascript
getY() : number;
```
**Remarks**
How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000d;
### setY(number) {#setY-number-}
Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.
```javascript
setY(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000d;
### getHeight() {#getHeight--}
Gets or sets the height of frame in units of 1/4000 of the chart area.
```javascript
getHeight() : number;
```
**Remarks**
How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000d;
### setHeight(number) {#setHeight-number-}
Gets or sets the height of frame in units of 1/4000 of the chart area.
```javascript
setHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000d;
### getWidth() {#getWidth--}
Gets or sets the width of frame in units of 1/4000 of the chart area.
```javascript
getWidth() : number;
```
**Remarks**
How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000d;
### setWidth(number) {#setWidth-number-}
Gets or sets the width of frame in units of 1/4000 of the chart area.
```javascript
setWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000d;
### getXRatioToChart() {#getXRatioToChart--}
Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area.
```javascript
getXRatioToChart() : number;
```
**Remarks**
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? XPixel = XRatioToChart * Chart.ChartObject.Width;
### setXRatioToChart(number) {#setXRatioToChart-number-}
Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area.
```javascript
setXRatioToChart(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? XPixel = XRatioToChart * Chart.ChartObject.Width;
### getYRatioToChart() {#getYRatioToChart--}
Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area.
```javascript
getYRatioToChart() : number;
```
**Remarks**
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? YPixel = YRatioToChart * Chart.ChartObject.Height;
### setYRatioToChart(number) {#setYRatioToChart-number-}
Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area.
```javascript
setYRatioToChart(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? YPixel = YRatioToChart * Chart.ChartObject.Height;
### getWidthRatioToChart() {#getWidthRatioToChart--}
Gets or sets the width of frame in units of ratio of the chart area.
```javascript
getWidthRatioToChart() : number;
```
**Remarks**
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;
### setWidthRatioToChart(number) {#setWidthRatioToChart-number-}
Gets or sets the width of frame in units of ratio of the chart area.
```javascript
setWidthRatioToChart(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;
### getHeightRatioToChart() {#getHeightRatioToChart--}
Gets or sets the height of frame in units of ratio of the chart area.
```javascript
getHeightRatioToChart() : number;
```
**Remarks**
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;
### setHeightRatioToChart(number) {#setHeightRatioToChart-number-}
Gets or sets the height of frame in units of ratio of the chart area.
```javascript
setHeightRatioToChart(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;
### getXPixel() {#getXPixel--}
Gets or sets the x coordinate of the upper left corner in units of Pixel.
```javascript
getXPixel() : number;
```
### setXPixel(number) {#setXPixel-number-}
Gets or sets the x coordinate of the upper left corner in units of Pixel.
```javascript
setXPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getYPixel() {#getYPixel--}
Gets or sets the y coordinate of the upper left corner in units of Pixel.
```javascript
getYPixel() : number;
```
### setYPixel(number) {#setYPixel-number-}
Gets or sets the y coordinate of the upper left corner in units of Pixel.
```javascript
setYPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getWidthPixel() {#getWidthPixel--}
Gets or sets the width of frame in units of Pixel.
```javascript
getWidthPixel() : number;
```
### setWidthPixel(number) {#setWidthPixel-number-}
Gets or sets the width of frame in units of Pixel.
```javascript
setWidthPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getHeightPixel() {#getHeightPixel--}
Gets or sets the height of frame in units of Pixel.
```javascript
getHeightPixel() : number;
```
### setHeightPixel(number) {#setHeightPixel-number-}
Gets or sets the height of frame in units of Pixel.
```javascript
setHeightPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### setPositionAuto() {#setPositionAuto--}
Set position of the frame to automatic
```javascript
setPositionAuto() : void;
```
### isAutoText() {#isAutoText--}
Indicates the text is auto generated.
```javascript
isAutoText() : boolean;
```
### setIsAutoText(boolean) {#setIsAutoText-boolean-}
Indicates the text is auto generated.
```javascript
setIsAutoText(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getLinkedSource() {#getLinkedSource--}
Gets and sets a reference to the worksheet.
```javascript
getLinkedSource() : string;
```
### setLinkedSource(string) {#setLinkedSource-string-}
Gets and sets a reference to the worksheet.
```javascript
setLinkedSource(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getDirectionType() {#getDirectionType--}
Gets and sets the direction of text.
```javascript
getDirectionType() : ChartTextDirectionType;
```
**Returns**
[ChartTextDirectionType](../charttextdirectiontype/)
### setDirectionType(ChartTextDirectionType) {#setDirectionType-charttextdirectiontype-}
Gets and sets the direction of text.
```javascript
setDirectionType(value: ChartTextDirectionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartTextDirectionType](../charttextdirectiontype/) | The value to set. |
### isTextWrapped() {#isTextWrapped--}
Gets or sets a value indicating whether the text is wrapped.
```javascript
isTextWrapped() : boolean;
```
### setIsTextWrapped(boolean) {#setIsTextWrapped-boolean-}
Gets or sets a value indicating whether the text is wrapped.
```javascript
setIsTextWrapped(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
