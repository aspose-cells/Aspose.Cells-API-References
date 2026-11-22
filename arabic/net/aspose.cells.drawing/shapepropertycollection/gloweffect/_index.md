---
title: "ShapePropertyCollection.GlowEffect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapePropertyCollection. تمثل كائن GlowEffect يحدد تأثير التوهج لعنصر المخطط أو الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shapepropertycollection/gloweffect/
---
## ShapePropertyCollection.GlowEffect property

تمثل كائن `GlowEffect` يحدد تأثير التوهج لعنصر المخطط أو الشكل.

```csharp
public GlowEffect GlowEffect { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShapePropertyCollectionPropertyGlowEffectDemo
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

            GlowEffect glowEffect = shapeProperties.GlowEffect;
            glowEffect.Size = 30;
            glowEffect.Color.Color = Color.Red;

            // تعيين ألوان السلسلة
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // احفظ المصنف
            workbook.Save("GlowEffectDemo.xlsx");            
        }
    }
}
```

### انظر أيضًا

* class [GlowEffect](../../gloweffect/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


