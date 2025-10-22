##DataLabels
Encapsulates a collection of all the DataLabel objects for the specified Series.
## DataLabels class
Encapsulates a collection of all the DataLabel objects for the specified Series.
```javascript
class DataLabels extends ChartTextFrame;
```
### Example
```javascript
const { Workbook, ChartType, LabelPositionType } = AsposeCells;
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
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(4);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(20);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);
//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 25, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Set the DataLabels in the chart
var datalabels;
for (var i = 0; i < chart.nSeries.count; i++) {
datalabels = chart.nSeries.get(i).dataLabels;
//Set the position of DataLabels
datalabels.position = LabelPositionType.InsideBase;
//Show the category name in the DataLabels
datalabels.setCategoryNameShown(true);
//Show the value in the DataLabels
datalabels.showValue = true;
//Not show the percentage in the DataLabels
datalabels.setPercentageShown(false);
//Not show the legend key.
datalabels.setLegendKeyShown(false);
}
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(ChartTextFrame)](#constructor-charttextframe-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [backgroundMode](#backgroundMode--)| BackgroundMode | Gets and sets the display mode of the background |
| [showValue](#showValue--)| boolean | Represents a specified chart's data label values display behavior. True displays the values. False to hide. |
| [showCellRange](#showCellRange--)| boolean | Indicates whether showing cell range as the data labels. |
| [showPercentage](#showPercentage--)| boolean | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. |
| [showBubbleSize](#showBubbleSize--)| boolean | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. |
| [showCategoryName](#showCategoryName--)| boolean | Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide. |
| [showSeriesName](#showSeriesName--)| boolean | Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide. |
| [showLegendKey](#showLegendKey--)| boolean | Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible. |
| [numberFormat](#numberFormat--)| string | Represents the format string for the DataLabels object. |
| [number](#number--)| number | Gets and sets the built-in number format. |
| [numberFormatLinked](#numberFormatLinked--)| boolean | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [separatorType](#separatorType--)| DataLabelsSeparatorType | Gets or sets the separator type used for the data labels on a chart. |
| [separatorValue](#separatorValue--)| string | Gets or sets the separator value used for the data labels on a chart. |
| [position](#position--)| LabelPositionType | Represents the position of the data label. |
| [isNeverOverlap](#isNeverOverlap--)| boolean | Indicates whether the datalabels display never overlap. (For Pie chart) |
| [shapeType](#shapeType--)| DataLabelShapeType | Gets or sets  shape type of data label. |
| [isInnerMode](#isInnerMode--)| boolean | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
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
| [applyFont()](#applyFont--)| Apply the font of the datalabels to all child nodes. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the text. |
| [getBorder()](#getBorder--)| Gets the <see cref="Line">border</see>. |
| [getArea()](#getArea--)| Gets the <see cref="Area">area</see>. |
| [isAutoText()](#isAutoText--)| Indicates the text is auto generated. |
| [setIsAutoText(boolean)](#setIsAutoText-boolean-)| Indicates the text is auto generated. |
| [getDirectionType()](#getDirectionType--)| Gets and sets the direction of text. |
| [setDirectionType(ChartTextDirectionType)](#setDirectionType-charttextdirectiontype-)| Gets and sets the direction of text. |
| [getText()](#getText--)| Gets or sets the text of data label. |
| [setText(string)](#setText-string-)| Gets or sets the text of data label. |
| [isTextWrapped()](#isTextWrapped--)| Gets or sets a value indicating whether the text is wrapped. |
| [setIsTextWrapped(boolean)](#setIsTextWrapped-boolean-)| Gets or sets a value indicating whether the text is wrapped. |
| [getFont()](#getFont--)| Gets the font of the DataLabels; |
| [getTextOptions()](#getTextOptions--)| Gets and sets the options of the text. |
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
| [getLinkedSource()](#getLinkedSource--)| Gets and sets a reference to the worksheet. |
| [setLinkedSource(string)](#setLinkedSource-string-)| Gets and sets a reference to the worksheet. |
### constructor(ChartTextFrame) {#constructor-charttextframe-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: ChartTextFrame);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ChartTextFrame | The parent object. |
### backgroundMode {#backgroundMode--}
Gets and sets the display mode of the background
```javascript
backgroundMode : BackgroundMode;
```
### showValue {#showValue--}
Represents a specified chart's data label values display behavior. True displays the values. False to hide.
```javascript
showValue : boolean;
```
### showCellRange {#showCellRange--}
Indicates whether showing cell range as the data labels.
```javascript
showCellRange : boolean;
```
### showPercentage {#showPercentage--}
Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.
```javascript
showPercentage : boolean;
```
### showBubbleSize {#showBubbleSize--}
Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.
```javascript
showBubbleSize : boolean;
```
### showCategoryName {#showCategoryName--}
Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide.
```javascript
showCategoryName : boolean;
```
### showSeriesName {#showSeriesName--}
Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide.
```javascript
showSeriesName : boolean;
```
### showLegendKey {#showLegendKey--}
Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible.
```javascript
showLegendKey : boolean;
```
### numberFormat {#numberFormat--}
Represents the format string for the DataLabels object.
```javascript
numberFormat : string;
```
### number {#number--}
Gets and sets the built-in number format.
```javascript
number : number;
```
### numberFormatLinked {#numberFormatLinked--}
True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).
```javascript
numberFormatLinked : boolean;
```
### separatorType {#separatorType--}
Gets or sets the separator type used for the data labels on a chart.
```javascript
separatorType : DataLabelsSeparatorType;
```
**Remarks**
To set custom separator, please set  the property [DataLabels.SeparatorType](../datalabels.separatortype/) as [DataLabelsSeparatorType.Custom](../datalabelsseparatortype.custom/) and then specify the expected value for [DataLabels.SeparatorValue](../datalabels.separatorvalue/).
### separatorValue {#separatorValue--}
Gets or sets the separator value used for the data labels on a chart.
```javascript
separatorValue : string;
```
### position {#position--}
Represents the position of the data label.
```javascript
position : LabelPositionType;
```
### isNeverOverlap {#isNeverOverlap--}
Indicates whether the datalabels display never overlap. (For Pie chart)
```javascript
isNeverOverlap : boolean;
```
### shapeType {#shapeType--}
Gets or sets  shape type of data label.
```javascript
shapeType : DataLabelShapeType;
```
### isInnerMode {#isInnerMode--}
Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.
```javascript
isInnerMode : boolean;
```
**Remarks**
Only for Xlsx file.
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
### applyFont() {#applyFont--}
Apply the font of the datalabels to all child nodes.
```javascript
applyFont() : void;
```
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
### getText() {#getText--}
Gets or sets the text of data label.
```javascript
getText() : string;
```
### setText(string) {#setText-string-}
Gets or sets the text of data label.
```javascript
setText(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
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
### getFont() {#getFont--}
Gets the font of the DataLabels;
```javascript
getFont() : Font;
```
**Returns**
[Font](../font/)
### getTextOptions() {#getTextOptions--}
Gets and sets the options of the text.
```javascript
getTextOptions() : TextOptions;
```
**Returns**
[TextOptions](../textoptions/)
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
