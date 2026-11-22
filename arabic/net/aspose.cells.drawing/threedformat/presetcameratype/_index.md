---
title: "ThreeDFormat.PresetCameraType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. يحصل على ويضبط نوع الكاميرا المسبق للتمدد"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/presetcameratype/
---
## ThreeDFormat.PresetCameraType property

يحصل ويضبط نوع كاميرا البثق المحددة مسبقًا.

```csharp
public PresetCameraType PresetCameraType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPresetCameraTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتوضيح تنسيق ثلاثي الأبعاد
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 200);
            
            // الحصول على ThreeDFormat الخاص بالشكل
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // عرض قيمة PresetCameraType الحالية
            Console.WriteLine("Current PresetCameraType: " + threeDFormat.PresetCameraType);

            // تعيين قيمة PresetCameraType جديدة
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveHeroicLeftFacing;

            // تطبيق بعض التنسيقات الثلاثية الأبعاد الإضافية لجعل التأثير مرئيًا
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // عرض قيمة PresetCameraType الجديدة
            Console.WriteLine("New PresetCameraType: " + threeDFormat.PresetCameraType);

            // احفظ المصنف لإظهار التأثير
            workbook.Save("ThreeDFormatPresetCameraTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PresetCameraType](../../presetcameratype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


