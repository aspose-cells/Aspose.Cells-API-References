---
title: "ThreeDFormat.Material"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. تمثل المادة المحددة مسبقًا التي تُدمج مع خصائص الإضاءة لتُعطي المظهر النهائي للشكل"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/material/
---
## ThreeDFormat.Material property

يمثل المادة المحددة مسبقًا التي تُدمج مع خصائص الإضاءة لتوفير المظهر والشعور النهائي للشكل.

```csharp
public PresetMaterialType Material { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyMaterialDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتوضيح تنسيق ثلاثي الأبعاد
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);
            shape.Text = "3D Material Demo";
            
            // الوصول إلى ThreeDFormat الخاص بالشكل
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // اعرض قيمة المادة الحالية
            Console.WriteLine("Current Material value: " + threeDFormat.Material);

            // حدد أنواع مواد مختلفة ولاحظ التأثيرات
            threeDFormat.Material = PresetMaterialType.Metal;
            Console.WriteLine("Material changed to Metal");

            threeDFormat.Material = PresetMaterialType.Plastic;
            Console.WriteLine("Material changed to Plastic");

            threeDFormat.Material = PresetMaterialType.Matte;
            Console.WriteLine("Material changed to Matte");

            // قم بتهيئة خصائص 3D الأخرى لرؤية تأثير المادة بشكل أفضل
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // حفظ المصنف مع تأثيرات ثلاثية الأبعاد
            workbook.Save("ThreeDFormatMaterialDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


