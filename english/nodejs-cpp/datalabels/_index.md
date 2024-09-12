---
title: DataLabels
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of all the DataLabel objects for the specified Series.
type: docs
url: /nodejs-cpp/datalabels/
---

## DataLabels class

Encapsulates a collection of all the DataLabel objects for the specified Series.

```javascript
class DataLabels extends ChartTextFrame;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(ChartTextFrame)](#constructor-charttextframe-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
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
| [getBackgroundMode()](#getBackgroundMode--)| Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| Gets and sets the display mode of the background |
| [getShowValue()](#getShowValue--)| Represents a specified chart's data label values display behavior. True displays the values. False to hide. |
| [setShowValue(boolean)](#setShowValue-boolean-)| Represents a specified chart's data label values display behavior. True displays the values. False to hide. |
| [getShowCellRange()](#getShowCellRange--)| Indicates whether showing cell range as the data labels. |
| [setShowCellRange(boolean)](#setShowCellRange-boolean-)| Indicates whether showing cell range as the data labels. |
| [getShowPercentage()](#getShowPercentage--)| Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. |
| [setShowPercentage(boolean)](#setShowPercentage-boolean-)| Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. |
| [getShowBubbleSize()](#getShowBubbleSize--)| Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. |
| [setShowBubbleSize(boolean)](#setShowBubbleSize-boolean-)| Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. |
| [getShowCategoryName()](#getShowCategoryName--)| Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide. |
| [setShowCategoryName(boolean)](#setShowCategoryName-boolean-)| Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide. |
| [getShowSeriesName()](#getShowSeriesName--)| Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide. |
| [setShowSeriesName(boolean)](#setShowSeriesName-boolean-)| Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide. |
| [getShowLegendKey()](#getShowLegendKey--)| Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible. |
| [setShowLegendKey(boolean)](#setShowLegendKey-boolean-)| Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible. |
| [get_NumberFormat()](#get_NumberFormat--)| Represents the format string for the DataLabels object. |
| [setNumberFormat(string)](#setNumberFormat-string-)| Represents the format string for the DataLabels object. |
| [getNumber()](#getNumber--)| Gets and sets the built-in number format. |
| [setNumber(number)](#setNumber-number-)| Gets and sets the built-in number format. |
| [getNumberFormatLinked()](#getNumberFormatLinked--)| True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [setNumberFormatLinked(boolean)](#setNumberFormatLinked-boolean-)| True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [getFont()](#getFont--)| Gets the font of the DataLabels; |
| [getSeparatorType()](#getSeparatorType--)| Gets or sets the separator type used for the data labels on a chart. |
| [setSeparatorType(DataLabelsSeparatorType)](#setSeparatorType-datalabelsseparatortype-)| Gets or sets the separator type used for the data labels on a chart. |
| [getSeparatorValue()](#getSeparatorValue--)| Gets or sets the separator value used for the data labels on a chart. |
| [setSeparatorValue(string)](#setSeparatorValue-string-)| Gets or sets the separator value used for the data labels on a chart. |
| [getPosition()](#getPosition--)| Represents the position of the data label. |
| [setPosition(LabelPositionType)](#setPosition-labelpositiontype-)| Represents the position of the data label. |
| [isNeverOverlap()](#isNeverOverlap--)| Indicates whether the datalabels display never overlap. (For Pie chart) |
| [setIsNeverOverlap(boolean)](#setIsNeverOverlap-boolean-)| Indicates whether the datalabels display never overlap. (For Pie chart) |
| [getShapeType()](#getShapeType--)| Gets or sets  shape type of data label. |
| [setShapeType(DataLabelShapeType)](#setShapeType-datalabelshapetype-)| Gets or sets  shape type of data label. |
| [applyFont()](#applyFont--)| Apply the font of the datalabels to all child nodes. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [isInnerMode()](#isInnerMode--)| Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [setIsInnerMode(boolean)](#setIsInnerMode-boolean-)| Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [getShadow()](#getShadow--)| True if the frame has a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| True if the frame has a shadow. |
| [getShapeProperties()](#getShapeProperties--)| Gets the [ShapeProperties](../shapeproperties/) object. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--)| Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [getDefaultX()](#getDefaultX--)| Represents x of default position |
| [getDefaultY()](#getDefaultY--)| Represents y of default position |
| [getDefaultWidth()](#getDefaultWidth--)| Represents width of default position |
| [getDefaultHeight()](#getDefaultHeight--)| Represents height of default position |
| [setPositionAuto()](#setPositionAuto--)| Set position of the frame to automatic |
| [isDeleted()](#isDeleted--)| Indicates whether this data labels is deleted. |
| [setIsDeleted(boolean)](#setIsDeleted-boolean-)| Indicates whether this data labels is deleted. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--)| Gets and sets the text horizontal alignment. |
| [setTextHorizontalAlignment(TextAlignmentType)](#setTextHorizontalAlignment-textalignmenttype-)| Gets and sets the text horizontal alignment. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--)| Gets or sets the text vertical alignment of text. |
| [setTextVerticalAlignment(TextAlignmentType)](#setTextVerticalAlignment-textalignmenttype-)| Gets or sets the text vertical alignment of text. |
| [getRotationAngle()](#getRotationAngle--)| Represents text rotation angle. |
| [setRotationAngle(number)](#setRotationAngle-number-)| Represents text rotation angle. |
| [isAutomaticRotation()](#isAutomaticRotation--)| Indicates whether the text of the chart is automatically rotated. |
| [getReadingOrder()](#getReadingOrder--)| Represents text reading order. |
| [setReadingOrder(TextDirectionType)](#setReadingOrder-textdirectiontype-)| Represents text reading order. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--)| Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [setIsResizeShapeToFitText(boolean)](#setIsResizeShapeToFitText-boolean-)| Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the text. |
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

### getBackgroundMode() {#getBackgroundMode--}

Gets and sets the display mode of the background

```javascript
getBackgroundMode() : BackgroundMode;
```


**Returns**

[BackgroundMode](../backgroundmode/)

### setBackgroundMode(BackgroundMode) {#setBackgroundMode-backgroundmode-}

Gets and sets the display mode of the background

```javascript
setBackgroundMode(value: BackgroundMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BackgroundMode](../backgroundmode/) | The value to set. |

### getShowValue() {#getShowValue--}

Represents a specified chart's data label values display behavior. True displays the values. False to hide.

```javascript
getShowValue() : boolean;
```


### setShowValue(boolean) {#setShowValue-boolean-}

Represents a specified chart's data label values display behavior. True displays the values. False to hide.

```javascript
setShowValue(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowCellRange() {#getShowCellRange--}

Indicates whether showing cell range as the data labels.

```javascript
getShowCellRange() : boolean;
```


### setShowCellRange(boolean) {#setShowCellRange-boolean-}

Indicates whether showing cell range as the data labels.

```javascript
setShowCellRange(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowPercentage() {#getShowPercentage--}

Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

```javascript
getShowPercentage() : boolean;
```


### setShowPercentage(boolean) {#setShowPercentage-boolean-}

Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

```javascript
setShowPercentage(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowBubbleSize() {#getShowBubbleSize--}

Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

```javascript
getShowBubbleSize() : boolean;
```


### setShowBubbleSize(boolean) {#setShowBubbleSize-boolean-}

Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

```javascript
setShowBubbleSize(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowCategoryName() {#getShowCategoryName--}

Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide.

```javascript
getShowCategoryName() : boolean;
```


### setShowCategoryName(boolean) {#setShowCategoryName-boolean-}

Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide.

```javascript
setShowCategoryName(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowSeriesName() {#getShowSeriesName--}

Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide.

```javascript
getShowSeriesName() : boolean;
```


### setShowSeriesName(boolean) {#setShowSeriesName-boolean-}

Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide.

```javascript
setShowSeriesName(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowLegendKey() {#getShowLegendKey--}

Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible.

```javascript
getShowLegendKey() : boolean;
```


### setShowLegendKey(boolean) {#setShowLegendKey-boolean-}

Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible.

```javascript
setShowLegendKey(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### get_NumberFormat() {#get_NumberFormat--}

Represents the format string for the DataLabels object.

```javascript
get_NumberFormat() : string;
```


### setNumberFormat(string) {#setNumberFormat-string-}

Represents the format string for the DataLabels object.

```javascript
setNumberFormat(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getNumber() {#getNumber--}

Gets and sets the built-in number format.

```javascript
getNumber() : number;
```


### setNumber(number) {#setNumber-number-}

Gets and sets the built-in number format.

```javascript
setNumber(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getNumberFormatLinked() {#getNumberFormatLinked--}

True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

```javascript
getNumberFormatLinked() : boolean;
```


### setNumberFormatLinked(boolean) {#setNumberFormatLinked-boolean-}

True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

```javascript
setNumberFormatLinked(value: boolean) : void;
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

### getSeparatorType() {#getSeparatorType--}

Gets or sets the separator type used for the data labels on a chart.

```javascript
getSeparatorType() : DataLabelsSeparatorType;
```


**Returns**

[DataLabelsSeparatorType](../datalabelsseparatortype/)

**Remarks**

To set custom separator, please set  the property [DataLabels.SeparatorType](../datalabels.separatortype/) as [DataLabels.SeparatorType](../datalabels.separatortype/) and then specify the expected value for [DataLabels.SeparatorType](../datalabels.separatortype/).

### setSeparatorType(DataLabelsSeparatorType) {#setSeparatorType-datalabelsseparatortype-}

Gets or sets the separator type used for the data labels on a chart.

```javascript
setSeparatorType(value: DataLabelsSeparatorType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DataLabelsSeparatorType](../datalabelsseparatortype/) | The value to set. |

**Remarks**

To set custom separator, please set  the property [DataLabels.SeparatorType](../datalabels.separatortype/) as [DataLabels.SeparatorType](../datalabels.separatortype/) and then specify the expected value for [DataLabels.SeparatorType](../datalabels.separatortype/).

### getSeparatorValue() {#getSeparatorValue--}

Gets or sets the separator value used for the data labels on a chart.

```javascript
getSeparatorValue() : string;
```


### setSeparatorValue(string) {#setSeparatorValue-string-}

Gets or sets the separator value used for the data labels on a chart.

```javascript
setSeparatorValue(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPosition() {#getPosition--}

Represents the position of the data label.

```javascript
getPosition() : LabelPositionType;
```


**Returns**

[LabelPositionType](../labelpositiontype/)

### setPosition(LabelPositionType) {#setPosition-labelpositiontype-}

Represents the position of the data label.

```javascript
setPosition(value: LabelPositionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LabelPositionType](../labelpositiontype/) | The value to set. |

### isNeverOverlap() {#isNeverOverlap--}

Indicates whether the datalabels display never overlap. (For Pie chart)

```javascript
isNeverOverlap() : boolean;
```


### setIsNeverOverlap(boolean) {#setIsNeverOverlap-boolean-}

Indicates whether the datalabels display never overlap. (For Pie chart)

```javascript
setIsNeverOverlap(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShapeType() {#getShapeType--}

Gets or sets  shape type of data label.

```javascript
getShapeType() : DataLabelShapeType;
```


**Returns**

[DataLabelShapeType](../datalabelshapetype/)

### setShapeType(DataLabelShapeType) {#setShapeType-datalabelshapetype-}

Gets or sets  shape type of data label.

```javascript
setShapeType(value: DataLabelShapeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DataLabelShapeType](../datalabelshapetype/) | The value to set. |

### applyFont() {#applyFont--}

Apply the font of the datalabels to all child nodes.

```javascript
applyFont() : void;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### isInnerMode() {#isInnerMode--}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.

```javascript
isInnerMode() : boolean;
```


**Remarks**

Only for Xlsx file.

### setIsInnerMode(boolean) {#setIsInnerMode-boolean-}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.

```javascript
setIsInnerMode(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for Xlsx file.

### getShadow() {#getShadow--}

True if the frame has a shadow.

```javascript
getShadow() : boolean;
```


### setShadow(boolean) {#setShadow-boolean-}

True if the frame has a shadow.

```javascript
setShadow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShapeProperties() {#getShapeProperties--}

Gets the [ShapeProperties](../shapeproperties/) object.

```javascript
getShapeProperties() : ShapePropertyCollection;
```


**Returns**

[ShapePropertyCollection](../shapepropertycollection/)

### isDefaultPosBeSet() {#isDefaultPosBeSet--}

Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

```javascript
isDefaultPosBeSet() : boolean;
```


### getDefaultX() {#getDefaultX--}

Represents x of default position

```javascript
getDefaultX() : number;
```


### getDefaultY() {#getDefaultY--}

Represents y of default position

```javascript
getDefaultY() : number;
```


### getDefaultWidth() {#getDefaultWidth--}

Represents width of default position

```javascript
getDefaultWidth() : number;
```


### getDefaultHeight() {#getDefaultHeight--}

Represents height of default position

```javascript
getDefaultHeight() : number;
```


### setPositionAuto() {#setPositionAuto--}

Set position of the frame to automatic

```javascript
setPositionAuto() : void;
```


### isDeleted() {#isDeleted--}

Indicates whether this data labels is deleted.

```javascript
isDeleted() : boolean;
```


### setIsDeleted(boolean) {#setIsDeleted-boolean-}

Indicates whether this data labels is deleted.

```javascript
setIsDeleted(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}

Gets and sets the text horizontal alignment.

```javascript
getTextHorizontalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setTextHorizontalAlignment(TextAlignmentType) {#setTextHorizontalAlignment-textalignmenttype-}

Gets and sets the text horizontal alignment.

```javascript
setTextHorizontalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### getTextVerticalAlignment() {#getTextVerticalAlignment--}

Gets or sets the text vertical alignment of text.

```javascript
getTextVerticalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setTextVerticalAlignment(TextAlignmentType) {#setTextVerticalAlignment-textalignmenttype-}

Gets or sets the text vertical alignment of text.

```javascript
setTextVerticalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### getRotationAngle() {#getRotationAngle--}

Represents text rotation angle.

```javascript
getRotationAngle() : number;
```


**Remarks**

<br>0: Not rotated.</br> <br>255: Top to Bottom.</br> <br>-90: Downward.</br> <br>90: Upward.</br>

### setRotationAngle(number) {#setRotationAngle-number-}

Represents text rotation angle.

```javascript
setRotationAngle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

<br>0: Not rotated.</br> <br>255: Top to Bottom.</br> <br>-90: Downward.</br> <br>90: Upward.</br>

### isAutomaticRotation() {#isAutomaticRotation--}

Indicates whether the text of the chart is automatically rotated.

```javascript
isAutomaticRotation() : boolean;
```


### getReadingOrder() {#getReadingOrder--}

Represents text reading order.

```javascript
getReadingOrder() : TextDirectionType;
```


**Returns**

[TextDirectionType](../textdirectiontype/)

### setReadingOrder(TextDirectionType) {#setReadingOrder-textdirectiontype-}

Represents text reading order.

```javascript
setReadingOrder(value: TextDirectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextDirectionType](../textdirectiontype/) | The value to set. |

### isResizeShapeToFitText() {#isResizeShapeToFitText--}

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

```javascript
isResizeShapeToFitText() : boolean;
```


### setIsResizeShapeToFitText(boolean) {#setIsResizeShapeToFitText-boolean-}

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

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

How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000;

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

How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000;

### getY() {#getY--}

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.

```javascript
getY() : number;
```


**Remarks**

How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000;

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

How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000;

### getHeight() {#getHeight--}

Gets or sets the height of frame in units of 1/4000 of the chart area.

```javascript
getHeight() : number;
```


**Remarks**

How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000;

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

How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000;

### getWidth() {#getWidth--}

Gets or sets the width of frame in units of 1/4000 of the chart area.

```javascript
getWidth() : number;
```


**Remarks**

How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000;

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

How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000;

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


