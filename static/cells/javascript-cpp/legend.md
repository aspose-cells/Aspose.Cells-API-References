##Legend
Encapsulates the object that represents the chart legend.
## Legend class
Encapsulates the object that represents the chart legend.
```javascript
class Legend extends ChartTextFrame;
```
### Example
```javascript
const { Workbook, ChartType, LegendPositionType } = AsposeCells;
//Set Legend's width and height
var workbook = new Workbook();
var sheetIndex = workbook.worksheets.add();
var worksheet = workbook.worksheets.get(sheetIndex);
var charts = worksheet.charts;
//Create a chart
var chart = charts.get(charts.add(ChartType.Column, 1, 1, 10, 10));
var legend = chart.getLegend();
//Legend is at right side of chart by default.
//If the legend is at left or right side of the chart, setting Legend.X property will not take effect.
//If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.
legend.y = 1500;
legend.width = 50;
legend.height = 50;
//Set legend's position
legend.position = LegendPositionType.Left;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(ChartTextFrame)](#constructor-charttextframe-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [position](#position--)| LegendPositionType | Gets or sets the legend position type. |
| [legendEntries](#legendEntries--)| LegendEntryCollection | Readonly. Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type. |
| [isOverLay](#isOverLay--)| boolean | Gets or sets whether showing the legend without overlapping the chart. |
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
| [getLegendLabels()](#getLegendLabels--)| Gets the labels of the legend entries after call Chart.Calculate() method. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the text. |
| [getBorder()](#getBorder--)| Gets the <see cref="Line">border</see>. |
| [getArea()](#getArea--)| Gets the <see cref="Area">area</see>. |
| [getTextOptions()](#getTextOptions--)| Gets and sets the options of the text. |
| [getFont()](#getFont--)| Gets a [Font](../font/) object of the specified ChartFrame object. |
| [getAutoScaleFont()](#getAutoScaleFont--)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| True if the text in the object changes font size when the object size changes. The default value is True. |
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
| [getText()](#getText--)| Gets or sets the text of a frame's title. |
| [setText(string)](#setText-string-)| Gets or sets the text of a frame's title. |
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
### position {#position--}
Gets or sets the legend position type.
```javascript
position : LegendPositionType;
```
**Remarks**
br>Default position is right.</br> <br>If the legend is at left or right side of the chart, setting Legend.X property will not take effect.</br> <br>If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.</br
### legendEntries {#legendEntries--}
Readonly. Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type.
```javascript
legendEntries : LegendEntryCollection;
```
### isOverLay {#isOverLay--}
Gets or sets whether showing the legend without overlapping the chart.
```javascript
isOverLay : boolean;
```
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
### getLegendLabels() {#getLegendLabels--}
Gets the labels of the legend entries after call Chart.Calculate() method.
```javascript
getLegendLabels() : string[];
```
**Returns**
string[]
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
### getText() {#getText--}
Gets or sets the text of a frame's title.
```javascript
getText() : string;
```
### setText(string) {#setText-string-}
Gets or sets the text of a frame's title.
```javascript
setText(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
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
