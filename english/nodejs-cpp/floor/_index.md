---
title: Floor
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents the floor of a 3D chart.
type: docs
url: /nodejs-cpp/floor/
---

## Floor class

Encapsulates the object that represents the floor of a 3-D chart.

```javascript
class Floor extends Area;
```


### Example
```javascript
const { License, Workbook, ChartType, Color, GradientPresetType, GradientStyleType } = require("aspose.cells.node");

//Instantiate the License class
var license = new License();
license.setLicense("input/Aspose.Cells.lic");

//Instantiate the workbook object
var workbook = new Workbook();
//Get cells collection
var cells = workbook.getWorksheets().get(0).getCells();
//Put values in cells
cells.get("A1").putValue(1);
cells.get("A2").putValue(2);
cells.get("A3").putValue(3);

//get charts colletion
var charts = workbook.getWorksheets().get(0).getCharts();
//add a new chart 
var index = charts.add(ChartType.Column3DStacked, 5, 0, 15, 5);
//get the newly added chart
var chart = charts.get(index);
//set charts nseries
chart.getNSeries().add("A1:A3", true);
//Show data labels
chart.getNSeries().get(0).getDataLabels().setShowValue(true);

//Get chart's floor
var floor = chart.getFloor();
//set floor's border as red
floor.getBorder().setColor(new Color(0xff, 0, 0));
//set fill format
floor.getFillFormat().setPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

//save the file
workbook.save("output/ChartsFloor.xls");
```
## Constructors

| Name | Description |
| --- | --- |
| [constructor(Area)](#constructor-area-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getBorder()](#getBorder--)| Gets or sets the border [Line](../line/). |
| [setBorder(Line)](#setBorder-line-)| Gets or sets the border [Line](../line/). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getBackgroundColor()](#getBackgroundColor--)| Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [setBackgroundColor(Color)](#setBackgroundColor-color-)| Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [getForegroundColor()](#getForegroundColor--)| Gets or sets the foreground [Color](../color/). |
| [setForegroundColor(Color)](#setForegroundColor-color-)| Gets or sets the foreground [Color](../color/). |
| [getFormatting()](#getFormatting--)| Represents the formatting of the area. |
| [setFormatting(FormattingType)](#setFormatting-formattingtype-)| Represents the formatting of the area. |
| [getInvertIfNegative()](#getInvertIfNegative--)| If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [setInvertIfNegative(boolean)](#setInvertIfNegative-boolean-)| If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [getFillFormat()](#getFillFormat--)| Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [getTransparency()](#getTransparency--)| Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |


### constructor(Area) {#constructor-area-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Area);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Area | The parent object. |

### getBorder() {#getBorder--}

Gets or sets the border [Line](../line/).

```javascript
getBorder() : Line;
```


**Returns**

[Line](../line/)

### setBorder(Line) {#setBorder-line-}

Gets or sets the border [Line](../line/).

```javascript
setBorder(value: Line) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Line](../line/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getBackgroundColor() {#getBackgroundColor--}

Gets or sets the background [Color](../color/) of the [Area](../area/).

```javascript
getBackgroundColor() : Color;
```


**Returns**

[Color](../color/)

### setBackgroundColor(Color) {#setBackgroundColor-color-}

Gets or sets the background [Color](../color/) of the [Area](../area/).

```javascript
setBackgroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getForegroundColor() {#getForegroundColor--}

Gets or sets the foreground [Color](../color/).

```javascript
getForegroundColor() : Color;
```


**Returns**

[Color](../color/)

### setForegroundColor(Color) {#setForegroundColor-color-}

Gets or sets the foreground [Color](../color/).

```javascript
setForegroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getFormatting() {#getFormatting--}

Represents the formatting of the area.

```javascript
getFormatting() : FormattingType;
```


**Returns**

[FormattingType](../formattingtype/)

### setFormatting(FormattingType) {#setFormatting-formattingtype-}

Represents the formatting of the area.

```javascript
setFormatting(value: FormattingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormattingType](../formattingtype/) | The value to set. |

### getInvertIfNegative() {#getInvertIfNegative--}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
getInvertIfNegative() : boolean;
```


### setInvertIfNegative(boolean) {#setInvertIfNegative-boolean-}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
setInvertIfNegative(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFillFormat() {#getFillFormat--}

Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.

```javascript
getFillFormat() : FillFormat;
```


**Returns**

[FillFormat](../fillformat/)

### getTransparency() {#getTransparency--}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
getTransparency() : number;
```


### setTransparency(number) {#setTransparency-number-}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
setTransparency(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |


