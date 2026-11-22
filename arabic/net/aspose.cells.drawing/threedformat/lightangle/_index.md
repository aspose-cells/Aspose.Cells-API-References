---
title: "ThreeDFormat.LightAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. تحصل وتضبط زاوية أضواء البثق"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/lightangle/
---
## ThreeDFormat.LightAngle property

يحصل ويضبط زاوية أضواء البثق.

```csharp
public double LightAngle { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightAngleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتوضيح تنسيق ثلاثي الأبعاد
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D Format Demo";
            
            // الوصول إلى ThreeDFormat الخاص بالشكل
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // اعرض القيمة الحالية لـ LightAngle
            Console.WriteLine("Current LightAngle value: " + threeDFormat.LightAngle);

            // اضبط قيمة LightAngle جديدة (0 إلى 359.9 درجة)
            threeDFormat.LightAngle = 45;
            Console.WriteLine("New LightAngle value: " + threeDFormat.LightAngle);

            // قم بتكوين خصائص ثلاثية الأبعاد أخرى لرؤية تأثير LightAngle
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // حفظ المصنف لرؤية التأثيرات
            workbook.Save("ThreeDFormatLightAngleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


