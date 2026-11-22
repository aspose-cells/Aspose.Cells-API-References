---
title: "الفئة ShapePropertyCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.ShapePropertyCollection. هذه الفئة تحدد خصائص الشكل البصري لعنصر مخطط أو شكل"
type: docs
url: /ar/net/aspose.cells.drawing/shapepropertycollection/
---
## ShapePropertyCollection class

هذه الفئة تحدد خصائص الشكل البصري لعنصر مخطط أو شكل.

```csharp
public class ShapePropertyCollection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Format3D](../../aspose.cells.drawing/shapepropertycollection/format3d/) { get; } | يمثل كائنًا [`Format3D`](./format3d/) يحدد خصائص الشكل ثلاثي الأبعاد لعنصر المخطط أو الشكل. |
| [GlowEffect](../../aspose.cells.drawing/shapepropertycollection/gloweffect/) { get; } | يمثل كائنًا [`GlowEffect`](./gloweffect/) يحدد تأثير التوهج لعنصر المخطط أو الشكل. |
| [ShadowEffect](../../aspose.cells.drawing/shapepropertycollection/shadoweffect/) { get; } | يمثل كائنًا [`ShadowEffect`](./shadoweffect/) يحدد تأثير الظل لعنصر المخطط أو الشكل. |
| [SoftEdgeRadius](../../aspose.cells.drawing/shapepropertycollection/softedgeradius/) { get; set; } | الحصول على وتعيين نصف قطر الضبابية لتطبيقه على الحواف، بوحدة النقاط. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ClearFormat3D](../../aspose.cells.drawing/shapepropertycollection/clearformat3d/)() | يمسح خصائص الشكل ثلاثي الأبعاد للشكل. |
| [ClearGlowEffect](../../aspose.cells.drawing/shapepropertycollection/cleargloweffect/)() | يمسح تأثير التوهج للشكل. |
| [ClearShadowEffect](../../aspose.cells.drawing/shapepropertycollection/clearshadoweffect/)() | يمسح تأثير الظل لعنصر المخطط أو الشكل. |
| [HasFormat3D](../../aspose.cells.drawing/shapepropertycollection/hasformat3d/)() | يشير إلى ما إذا كان الشكل يحتوي على بيانات تنسيق ثلاثي الأبعاد. |
| [HasGlowEffect](../../aspose.cells.drawing/shapepropertycollection/hasgloweffect/)() | يشير إلى ما إذا كان الشكل يحتوي على بيانات تأثير التوهج. |
| [HasShadowEffect](../../aspose.cells.drawing/shapepropertycollection/hasshadoweffect/)() | يشير إلى ما إذا كان الشكل يحتوي على بيانات تأثير الظل. |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePropertyCollectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مخطط تجريبي
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            chart.NSeries.Add("B1:B2", true);
            chart.NSeries.CategoryData = "A1:A2";

            // الوصول إلى خصائص الشكل للسلسلة الأولى
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // تكوين تنسيق ثلاثي الأبعاد والحدب
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;
            
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;
            
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            // تعيين ألوان السلسلة
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // احفظ المصنف
            workbook.Save("ShapePropertyCollectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


