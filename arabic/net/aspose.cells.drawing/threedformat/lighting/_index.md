---
title: "ThreeDFormat.Lighting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. يسترجع ويعيّن نوع rig الإضاءة"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/lighting/
---
## ThreeDFormat.Lighting property

يحصل ويضبط نوع نظام الإضاءة.

```csharp
public LightRigType Lighting { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتوضيح تنسيق ثلاثي الأبعاد
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 200);
            shape.Text = "3D Lighting Demo";
            
            // الحصول على ThreeDFormat الخاص بالشكل
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // اعرض قيمة الإضاءة الحالية
            Console.WriteLine("Current Lighting value: " + threeDFormat.Lighting);

            // حدد أنواع إضاءة مختلفة ولاحظ التأثيرات
            threeDFormat.Lighting = LightRigType.BrightRoom;
            Console.WriteLine("Changed to BrightRoom lighting");

            // طبق بعض خصائص 3D الأخرى لرؤية تأثير الإضاءة بشكل أفضل
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;

            // احفظ باستخدام نوع الإضاءة الأول
            workbook.Save("BrightRoomLighting.xlsx");

            // غيّر إلى نوع إضاءة آخر
            threeDFormat.Lighting = LightRigType.Sunset;
            Console.WriteLine("Changed to Sunset lighting");
            workbook.Save("SunsetLighting.xlsx");

            // غيّر إلى نوع إضاءة ثالث
            threeDFormat.Lighting = LightRigType.ThreePoint;
            Console.WriteLine("Changed to ThreePoint lighting");
            workbook.Save("ThreePointLighting.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [LightRigType](../../lightrigtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


