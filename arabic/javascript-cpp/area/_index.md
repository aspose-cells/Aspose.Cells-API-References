---
title: Area
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /ar/javascript-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//إنشاء كائن Workbook
var workbook = new Workbook();
//إضافة ورقة عمل جديدة إلى كائن Workbook
var sheetIndex = workbook.worksheets.add();
//الحصول على مرجع ورقة العمل المضافة حديثًا بتمرير فهرس الورقة الخاص بها
var worksheet = workbook.worksheets.get(sheetIndex);
//إضافة قيمة عينة إلى الخلية "A1"
worksheet.cells.get("A1").putValue(50);
//إضافة قيمة عينة إلى الخلية "A2"
worksheet.cells.get("A2").putValue(100);
//إضافة قيمة عينة إلى الخلية "A3"
worksheet.cells.get("A3").putValue(150);
//إضافة قيمة عينة إلى الخلية "B1"
worksheet.cells.get("B1").putValue(60);
//إضافة قيمة عينة إلى الخلية "B2"
worksheet.cells.get("B2").putValue(32);
//إضافة قيمة عينة إلى الخلية "B3"
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
var uint8Array = workbook.save(SaveFormat.Excel97To2003);
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
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//إنشاء كائن Workbook
var workbook = new Workbook();
//إضافة ورقة عمل جديدة إلى كائن Workbook
var sheetIndex = workbook.worksheets.add();
//الحصول على مرجع ورقة العمل المضافة حديثًا بتمرير فهرس الورقة الخاص بها
var worksheet = workbook.worksheets.get(sheetIndex);
//إضافة قيمة عينة إلى الخلية "A1"
worksheet.cells.get("A1").putValue(50);
//إضافة قيمة عينة إلى الخلية "A2"
worksheet.cells.get("A2").putValue(-100);
//إضافة قيمة عينة إلى الخلية "A3"
worksheet.cells.get("A3").putValue(150);
//إضافة مخطط إلى ورقة العمل
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//الوصول إلى نسخة المخطط المضاف حديثًا
var chart = worksheet.charts.get(chartIndex);
//إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "A3"
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//تعيين لون المقدمة لمنطقة السلسلة الأولى NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//تعيين لون الخلفية لمنطقة السلسلة الأولى NSeries.
//لون المنطقة المعروضة للنقطة الثانية في المخطط سيكون لون الخلفية.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//حفظ ملف Excel
var uint8Array = workbook.save(SaveFormat.Excel97To2003);
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



