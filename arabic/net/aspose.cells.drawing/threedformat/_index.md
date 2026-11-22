---
title: "الفئة ThreeDFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.ThreeDFormat. تمثل تنسيقًا ثلاثي الأبعاد للشكل"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/
---
## ThreeDFormat class

يمثل تنسيق الشكل ثلاثي الأبعاد.

```csharp
public class ThreeDFormat
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BottomBevelHeight](../../aspose.cells.drawing/threedformat/bottombevelheight/) { get; set; } | يحصل ويضبط ارتفاع الحافة السفلية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط. |
| [BottomBevelType](../../aspose.cells.drawing/threedformat/bottombeveltype/) { get; set; } | يحصل ويضبط نوع الحافة السفلية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط. |
| [BottomBevelWidth](../../aspose.cells.drawing/threedformat/bottombevelwidth/) { get; set; } | يحصل ويضبط عرض الحافة السفلية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط. |
| [ContourColor](../../aspose.cells.drawing/threedformat/contourcolor/) { get; set; } | يحصل ويضبط لون الخط المحيط على الشكل. |
| [ContourWidth](../../aspose.cells.drawing/threedformat/contourwidth/) { get; set; } | يحصل ويضبط عرض الخط المحيط على الشكل، بوحدة النقاط. |
| [ExtrusionColor](../../aspose.cells.drawing/threedformat/extrusioncolor/) { get; set; } | يحصل على لون البثق على الشكل. |
| [ExtrusionHeight](../../aspose.cells.drawing/threedformat/extrusionheight/) { get; set; } | يحصل ويضبط ارتفاع البثق المطبق على الشكل، بوحدة النقاط. |
| [LightAngle](../../aspose.cells.drawing/threedformat/lightangle/) { get; set; } | يحصل ويضبط زاوية أضواء البثق. |
| [Lighting](../../aspose.cells.drawing/threedformat/lighting/) { get; set; } | يحصل ويضبط نوع نظام الإضاءة. |
| [LightingDirection](../../aspose.cells.drawing/threedformat/lightingdirection/) { get; set; } | يحصل ويضبط الاتجاه الذي يُوجه منه نظام الإضاءة بالنسبة للمشهد. |
| [Material](../../aspose.cells.drawing/threedformat/material/) { get; set; } | يمثل المادة المحددة مسبقًا التي تُدمج مع خصائص الإضاءة لتوفير المظهر والشعور النهائي للشكل. |
| [Perspective](../../aspose.cells.drawing/threedformat/perspective/) { get; set; } | يحصل ويضبط الزاوية التي يمكن من خلالها عرض كائن ThreeDFormat. |
| [PresetCameraType](../../aspose.cells.drawing/threedformat/presetcameratype/) { get; set; } | يحصل ويضبط نوع كاميرا البثق المحددة مسبقًا. |
| [RotationX](../../aspose.cells.drawing/threedformat/rotationx/) { get; set; } | يحصل ويضبط دوران الشكل المُبثق حول المحور x بالدرجات. |
| [RotationY](../../aspose.cells.drawing/threedformat/rotationy/) { get; set; } | يحصل ويضبط دوران الشكل المُبثق حول المحور y بالدرجات. |
| [RotationZ](../../aspose.cells.drawing/threedformat/rotationz/) { get; set; } | يحصل ويضبط دوران الشكل المُبثق حول المحور z بالدرجات. |
| [TopBevelHeight](../../aspose.cells.drawing/threedformat/topbevelheight/) { get; set; } | يحصل ويضبط ارتفاع الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط. |
| [TopBevelType](../../aspose.cells.drawing/threedformat/topbeveltype/) { get; set; } | يحصل على ويضبط نوع الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط. |
| [TopBevelWidth](../../aspose.cells.drawing/threedformat/topbevelwidth/) { get; set; } | يحصل على ويضبط عرض الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط. |
| [Z](../../aspose.cells.drawing/threedformat/z/) { get; set; } | يحدد المسافة من الأرض للشكل ثلاثي الأبعاد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/threedformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/threedformat/gethashcode/)() | يحصل على قيمة التجزئة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassThreeDFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 210, 210, 200, 200);
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.ExtrusionHeight = 20;

            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


