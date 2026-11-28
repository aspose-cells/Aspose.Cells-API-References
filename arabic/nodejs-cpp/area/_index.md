---
title: Area
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /ar/nodejs-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//إنشاء كائن Workbook.
var workbook = new Workbook();
//إضافة ورقة عمل جديدة إلى كائن المصنف
var sheetIndex = workbook.worksheets.add();
//الحصول على مرجع ورقة العمل المضافة حديثًا بتمرير فهرسها
var worksheet = workbook.worksheets.get(sheetIndex);
//إضافة قيمة نموذجية إلى الخلية "A1"
worksheet.cells.get("A1").putValue(50);
//إضافة قيمة نموذجية إلى الخلية "A2"
worksheet.cells.get("A2").putValue(100);
//إضافة قيمة نموذجية إلى الخلية "A3"
worksheet.cells.get("A3").putValue(150);
//إضافة قيمة نموذجية إلى الخلية "B1"
worksheet.cells.get("B1").putValue(60);
//إضافة قيمة نموذجية إلى الخلية "B2"
worksheet.cells.get("B2").putValue(32);
//إضافة قيمة نموذجية إلى الخلية "B3"
worksheet.cells.get("B3").putValue(50);
//إضافة مخطط إلى ورقة العمل
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//الوصول إلى نسخة المخطط المضاف حديثًا
var chart = worksheet.charts.get(chartIndex);
//إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B3"
chart.nSeries.add("A1:B3", true);
//تعيين لون المقدمة لمنطقة الرسم
chart.plotArea.getArea().foregroundColor = Color.Blue;
//تعيين لون المقدمة لمنطقة المخطط
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//تعيين لون المقدمة لمنطقة السلسلة الأولى NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//تعيين لون المقدمة لمنطقة النقطة الأولى في السلسلة NSeries
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//حفظ ملف Excel
workbook.save("output/DrawingArea.xls");
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [backgroundColor](#backgroundColor--)| Color | Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [foregroundColor](#foregroundColor--)| Color | Gets or sets the foreground [Color](../color/). |
| [formatting](#formatting--)| FormattingType | Represents the formatting of the area. |
| [invertIfNegative](#invertIfNegative--)| boolean | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [fillFormat](#fillFormat--)| FillFormat | Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |

## Methods

| Method | Description |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [setBackgroundColor(Color)](#setBackgroundColor-color-)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [getForegroundColor()](#getForegroundColor--)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/). |
| [setForegroundColor(Color)](#setForegroundColor-color-)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/). |
| [getFormatting()](#getFormatting--)| <b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area. |
| [setFormatting(FormattingType)](#setFormatting-formattingtype-)| <b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area. |
| [getInvertIfNegative()](#getInvertIfNegative--)| <b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [setInvertIfNegative(boolean)](#setInvertIfNegative-boolean-)| <b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [getFillFormat()](#getFillFormat--)| <b>@deprecated.</b> Please use the 'fillFormat' property instead. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### backgroundColor {#backgroundColor--}

Gets or sets the background [Color](../color/) of the [Area](../area/).

```javascript
backgroundColor : Color;
```


### foregroundColor {#foregroundColor--}

Gets or sets the foreground [Color](../color/).

```javascript
foregroundColor : Color;
```


### formatting {#formatting--}

Represents the formatting of the area.

```javascript
formatting : FormattingType;
```


### invertIfNegative {#invertIfNegative--}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
invertIfNegative : boolean;
```


**Example**
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//إنشاء كائن Workbook.
var workbook = new Workbook();
//إضافة ورقة عمل جديدة إلى كائن المصنف
var sheetIndex = workbook.worksheets.add();
//الحصول على مرجع ورقة العمل المضافة حديثًا بتمرير فهرسها
var worksheet = workbook.worksheets.get(sheetIndex);
//إضافة قيمة نموذجية إلى الخلية "A1"
worksheet.cells.get("A1").putValue(50);
//إضافة قيمة نموذجية إلى الخلية "A2"
worksheet.cells.get("A2").putValue(-100);
//إضافة قيمة نموذجية إلى الخلية "A3"
worksheet.cells.get("A3").putValue(150);
//إضافة مخطط إلى ورقة العمل
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//الوصول إلى نسخة المخطط المضاف حديثًا
var chart = worksheet.charts.get(chartIndex);
//إضافة NSeries (مصدر بيانات المخطط) إلى المخطط الممتد من الخلية "A1" إلى "A3"
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//تعيين لون المقدمة لمنطقة السلسلة الأولى NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//تعيين لون الخلفية لمنطقة السلسلة الأولى NSeries.
//لون المنطقة المعروضة للنقطة الثانية في المخطط سيكون لون الخلفية.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//حفظ ملف Excel
workbook.save("output/DrawingAreaInverseIfNegative.xls");
```

### fillFormat {#fillFormat--}

Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.

```javascript
fillFormat : FillFormat;
```


### transparency {#transparency--}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
transparency : number;
```


### getBackgroundColor() {#getBackgroundColor--}

<b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/).

```javascript
getBackgroundColor() : Color;
```


**Returns**

[Color](../color/)

### setBackgroundColor(Color) {#setBackgroundColor-color-}

<b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/).

```javascript
setBackgroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getForegroundColor() {#getForegroundColor--}

<b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/).

```javascript
getForegroundColor() : Color;
```


**Returns**

[Color](../color/)

### setForegroundColor(Color) {#setForegroundColor-color-}

<b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/).

```javascript
setForegroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getFormatting() {#getFormatting--}

<b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area.

```javascript
getFormatting() : FormattingType;
```


**Returns**

[FormattingType](../formattingtype/)

### setFormatting(FormattingType) {#setFormatting-formattingtype-}

<b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area.

```javascript
setFormatting(value: FormattingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormattingType](../formattingtype/) | The value to set. |

### getInvertIfNegative() {#getInvertIfNegative--}

<b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
getInvertIfNegative() : boolean;
```


### setInvertIfNegative(boolean) {#setInvertIfNegative-boolean-}

<b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
setInvertIfNegative(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFillFormat() {#getFillFormat--}

<b>@deprecated.</b> Please use the 'fillFormat' property instead. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.

```javascript
getFillFormat() : FillFormat;
```


**Returns**

[FillFormat](../fillformat/)

### getTransparency() {#getTransparency--}

<b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
getTransparency() : number;
```


### setTransparency(number) {#setTransparency-number-}

<b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
setTransparency(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



