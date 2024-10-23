---
title: Line
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents the line format.
type: docs
url: /nodejs-cpp/line/
---

## Line class

Encapsulates the object that represents the line format.

```javascript
class Line;
```


### Example
```javascript
const { Workbook, ChartType, LineType, ChartMarkerType, WeightType } = require("aspose.cells.node");

var workbook = new Workbook();
var cells = workbook.getWorksheets().get(0).getCells();
cells.get("a1").putValue(2);
cells.get("a2").putValue(5);
cells.get("a3").putValue(3);
cells.get("a4").putValue(6);
cells.get("b1").putValue(4);
cells.get("b2").putValue(3);
cells.get("b3").putValue(6);
cells.get("b4").putValue(7);
var chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.Column, 11, 0, 27, 10);
var chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
chart.getNSeries().add("A1:B4", true);
//Applying a dotted line style on the lines of an NSeries
chart.getNSeries().get(0).getBorder().setStyle(LineType.Dot);
//Applying a triangular marker style on the data markers of an NSeries
chart.getNSeries().get(0).getMarker().setMarkerStyle(ChartMarkerType.Triangle);
//Setting the weight of all lines in an NSeries to medium
chart.getNSeries().get(0).getBorder().setWeight(WeightType.MediumLine);
```
## Methods

| Method | Description |
| --- | --- |
| [getCompoundType()](#getCompoundType--)| Specifies the compound line type |
| [setCompoundType(MsoLineStyle)](#setCompoundType-msolinestyle-)| Specifies the compound line type |
| [getDashType()](#getDashType--)| Specifies the dash line type |
| [setDashType(MsoLineDashStyle)](#setDashType-msolinedashstyle-)| Specifies the dash line type |
| [getCapType()](#getCapType--)| Specifies the ending caps. |
| [setCapType(LineCapType)](#setCapType-linecaptype-)| Specifies the ending caps. |
| [getJoinType()](#getJoinType--)| Specifies the joining caps. |
| [setJoinType(LineJoinType)](#setJoinType-linejointype-)| Specifies the joining caps. |
| [getBeginType()](#getBeginType--)| Specifies an arrowhead for the begin of a line. |
| [setBeginType(MsoArrowheadStyle)](#setBeginType-msoarrowheadstyle-)| Specifies an arrowhead for the begin of a line. |
| [getEndType()](#getEndType--)| Specifies an arrowhead for the end of a line. |
| [setEndType(MsoArrowheadStyle)](#setEndType-msoarrowheadstyle-)| Specifies an arrowhead for the end of a line. |
| [getBeginArrowLength()](#getBeginArrowLength--)| Specifies the length of the arrowhead for the begin of a line. |
| [setBeginArrowLength(MsoArrowheadLength)](#setBeginArrowLength-msoarrowheadlength-)| Specifies the length of the arrowhead for the begin of a line. |
| [getEndArrowLength()](#getEndArrowLength--)| Specifies the length of the arrowhead for the end of a line. |
| [setEndArrowLength(MsoArrowheadLength)](#setEndArrowLength-msoarrowheadlength-)| Specifies the length of the arrowhead for the end of a line. |
| [getBeginArrowWidth()](#getBeginArrowWidth--)| Specifies the width of the arrowhead for the begin of a line. |
| [setBeginArrowWidth(MsoArrowheadWidth)](#setBeginArrowWidth-msoarrowheadwidth-)| Specifies the width of the arrowhead for the begin of a line. |
| [getEndArrowWidth()](#getEndArrowWidth--)| Specifies the width of the arrowhead for the end of a line. |
| [setEndArrowWidth(MsoArrowheadWidth)](#setEndArrowWidth-msoarrowheadwidth-)| Specifies the width of the arrowhead for the end of a line. |
| [getThemeColor()](#getThemeColor--)| Gets and sets the theme color. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| Gets and sets the theme color. |
| [getColor()](#getColor--)| Represents the [Color](../color/) of the line. |
| [setColor(Color)](#setColor-color-)| Represents the [Color](../color/) of the line. |
| [getTransparency()](#getTransparency--)| Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [getStyle()](#getStyle--)| Represents the style of the line. |
| [setStyle(LineType)](#setStyle-linetype-)| Represents the style of the line. |
| [getWeight()](#getWeight--)| Gets or sets the [WeightType](../weighttype/) of the line. |
| [setWeight(WeightType)](#setWeight-weighttype-)| Gets or sets the [WeightType](../weighttype/) of the line. |
| [getWeightPt()](#getWeightPt--)| Gets or sets the weight of the line in unit of points. |
| [setWeightPt(number)](#setWeightPt-number-)| Gets or sets the weight of the line in unit of points. |
| [getWeightPx()](#getWeightPx--)| Gets or sets the weight of the line in unit of pixels. |
| [setWeightPx(number)](#setWeightPx-number-)| Gets or sets the weight of the line in unit of pixels. |
| [getFormattingType()](#getFormattingType--)| Gets or sets format type. |
| [setFormattingType(ChartLineFormattingType)](#setFormattingType-chartlineformattingtype-)| Gets or sets format type. |
| [isAutomaticColor()](#isAutomaticColor--)| Indicates whether the color of line is automatic assigned. |
| [isVisible()](#isVisible--)| Represents whether the line is visible. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| Represents whether the line is visible. |
| [isAuto()](#isAuto--)| Indicates whether this line style is auto assigned. |
| [setIsAuto(boolean)](#setIsAuto-boolean-)| Indicates whether this line style is auto assigned. |
| [getGradientFill()](#getGradientFill--)| Represents gradient fill. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getCompoundType() {#getCompoundType--}

Specifies the compound line type

```javascript
getCompoundType() : MsoLineStyle;
```


**Returns**

[MsoLineStyle](../msolinestyle/)

### setCompoundType(MsoLineStyle) {#setCompoundType-msolinestyle-}

Specifies the compound line type

```javascript
setCompoundType(value: MsoLineStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineStyle](../msolinestyle/) | The value to set. |

### getDashType() {#getDashType--}

Specifies the dash line type

```javascript
getDashType() : MsoLineDashStyle;
```


**Returns**

[MsoLineDashStyle](../msolinedashstyle/)

### setDashType(MsoLineDashStyle) {#setDashType-msolinedashstyle-}

Specifies the dash line type

```javascript
setDashType(value: MsoLineDashStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineDashStyle](../msolinedashstyle/) | The value to set. |

### getCapType() {#getCapType--}

Specifies the ending caps.

```javascript
getCapType() : LineCapType;
```


**Returns**

[LineCapType](../linecaptype/)

### setCapType(LineCapType) {#setCapType-linecaptype-}

Specifies the ending caps.

```javascript
setCapType(value: LineCapType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineCapType](../linecaptype/) | The value to set. |

### getJoinType() {#getJoinType--}

Specifies the joining caps.

```javascript
getJoinType() : LineJoinType;
```


**Returns**

[LineJoinType](../linejointype/)

### setJoinType(LineJoinType) {#setJoinType-linejointype-}

Specifies the joining caps.

```javascript
setJoinType(value: LineJoinType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineJoinType](../linejointype/) | The value to set. |

### getBeginType() {#getBeginType--}

Specifies an arrowhead for the begin of a line.

```javascript
getBeginType() : MsoArrowheadStyle;
```


**Returns**

[MsoArrowheadStyle](../msoarrowheadstyle/)

### setBeginType(MsoArrowheadStyle) {#setBeginType-msoarrowheadstyle-}

Specifies an arrowhead for the begin of a line.

```javascript
setBeginType(value: MsoArrowheadStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |

### getEndType() {#getEndType--}

Specifies an arrowhead for the end of a line.

```javascript
getEndType() : MsoArrowheadStyle;
```


**Returns**

[MsoArrowheadStyle](../msoarrowheadstyle/)

### setEndType(MsoArrowheadStyle) {#setEndType-msoarrowheadstyle-}

Specifies an arrowhead for the end of a line.

```javascript
setEndType(value: MsoArrowheadStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |

### getBeginArrowLength() {#getBeginArrowLength--}

Specifies the length of the arrowhead for the begin of a line.

```javascript
getBeginArrowLength() : MsoArrowheadLength;
```


**Returns**

[MsoArrowheadLength](../msoarrowheadlength/)

### setBeginArrowLength(MsoArrowheadLength) {#setBeginArrowLength-msoarrowheadlength-}

Specifies the length of the arrowhead for the begin of a line.

```javascript
setBeginArrowLength(value: MsoArrowheadLength) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |

### getEndArrowLength() {#getEndArrowLength--}

Specifies the length of the arrowhead for the end of a line.

```javascript
getEndArrowLength() : MsoArrowheadLength;
```


**Returns**

[MsoArrowheadLength](../msoarrowheadlength/)

### setEndArrowLength(MsoArrowheadLength) {#setEndArrowLength-msoarrowheadlength-}

Specifies the length of the arrowhead for the end of a line.

```javascript
setEndArrowLength(value: MsoArrowheadLength) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |

### getBeginArrowWidth() {#getBeginArrowWidth--}

Specifies the width of the arrowhead for the begin of a line.

```javascript
getBeginArrowWidth() : MsoArrowheadWidth;
```


**Returns**

[MsoArrowheadWidth](../msoarrowheadwidth/)

### setBeginArrowWidth(MsoArrowheadWidth) {#setBeginArrowWidth-msoarrowheadwidth-}

Specifies the width of the arrowhead for the begin of a line.

```javascript
setBeginArrowWidth(value: MsoArrowheadWidth) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |

### getEndArrowWidth() {#getEndArrowWidth--}

Specifies the width of the arrowhead for the end of a line.

```javascript
getEndArrowWidth() : MsoArrowheadWidth;
```


**Returns**

[MsoArrowheadWidth](../msoarrowheadwidth/)

### setEndArrowWidth(MsoArrowheadWidth) {#setEndArrowWidth-msoarrowheadwidth-}

Specifies the width of the arrowhead for the end of a line.

```javascript
setEndArrowWidth(value: MsoArrowheadWidth) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |

### getThemeColor() {#getThemeColor--}

Gets and sets the theme color.

```javascript
getThemeColor() : ThemeColor;
```


**Returns**

[ThemeColor](../themecolor/)

**Remarks**

If the foreground color is not a theme color, NULL will be returned.

### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}

Gets and sets the theme color.

```javascript
setThemeColor(value: ThemeColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../themecolor/) | The value to set. |

**Remarks**

If the foreground color is not a theme color, NULL will be returned.

### getColor() {#getColor--}

Represents the [Color](../color/) of the line.

```javascript
getColor() : Color;
```


**Returns**

[Color](../color/)

### setColor(Color) {#setColor-color-}

Represents the [Color](../color/) of the line.

```javascript
setColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getTransparency() {#getTransparency--}

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
getTransparency() : number;
```


### setTransparency(number) {#setTransparency-number-}

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
setTransparency(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getStyle() {#getStyle--}

Represents the style of the line.

```javascript
getStyle() : LineType;
```


**Returns**

[LineType](../linetype/)

### setStyle(LineType) {#setStyle-linetype-}

Represents the style of the line.

```javascript
setStyle(value: LineType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineType](../linetype/) | The value to set. |

### getWeight() {#getWeight--}

Gets or sets the [WeightType](../weighttype/) of the line.

```javascript
getWeight() : WeightType;
```


**Returns**

[WeightType](../weighttype/)

### setWeight(WeightType) {#setWeight-weighttype-}

Gets or sets the [WeightType](../weighttype/) of the line.

```javascript
setWeight(value: WeightType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WeightType](../weighttype/) | The value to set. |

### getWeightPt() {#getWeightPt--}

Gets or sets the weight of the line in unit of points.

```javascript
getWeightPt() : number;
```


### setWeightPt(number) {#setWeightPt-number-}

Gets or sets the weight of the line in unit of points.

```javascript
setWeightPt(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWeightPx() {#getWeightPx--}

Gets or sets the weight of the line in unit of pixels.

```javascript
getWeightPx() : number;
```


### setWeightPx(number) {#setWeightPx-number-}

Gets or sets the weight of the line in unit of pixels.

```javascript
setWeightPx(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFormattingType() {#getFormattingType--}

Gets or sets format type.

```javascript
getFormattingType() : ChartLineFormattingType;
```


**Returns**

[ChartLineFormattingType](../chartlineformattingtype/)

### setFormattingType(ChartLineFormattingType) {#setFormattingType-chartlineformattingtype-}

Gets or sets format type.

```javascript
setFormattingType(value: ChartLineFormattingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartLineFormattingType](../chartlineformattingtype/) | The value to set. |

### isAutomaticColor() {#isAutomaticColor--}

Indicates whether the color of line is automatic assigned.

```javascript
isAutomaticColor() : boolean;
```


### isVisible() {#isVisible--}

Represents whether the line is visible.

```javascript
isVisible() : boolean;
```


### setIsVisible(boolean) {#setIsVisible-boolean-}

Represents whether the line is visible.

```javascript
setIsVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isAuto() {#isAuto--}

Indicates whether this line style is auto assigned.

```javascript
isAuto() : boolean;
```


### setIsAuto(boolean) {#setIsAuto-boolean-}

Indicates whether this line style is auto assigned.

```javascript
setIsAuto(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getGradientFill() {#getGradientFill--}

Represents gradient fill.

```javascript
getGradientFill() : GradientFill;
```


**Returns**

[GradientFill](../gradientfill/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



