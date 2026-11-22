---
title: "فئة DrawObjectEventHandler"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Rendering.DrawObjectEventHandler. واجهة للحصول على DrawObject و Bound أثناء التصيير"
type: docs
url: /ar/net/aspose.cells.rendering/drawobjecteventhandler/
---
## DrawObjectEventHandler class

واجهة للحصول على DrawObject و Bound عند التصيير.

```csharp
public abstract class DrawObjectEventHandler
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [Draw](../../aspose.cells.rendering/drawobjecteventhandler/draw/)(DrawObject, float, float, float, float) | تنفذ هذه الواجهة للحصول على DrawObject و Bound أثناء التصيير. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassDrawObjectEventHandlerDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(12345);
            worksheet.Shapes.AddRectangle(5, 5, 50, 100, 200, 300); // Added missing parameter

            // إنشاء خيارات حفظ PDF مع معالج تصيير مخصص
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectHandler();

            // حفظ المصنف إلى PDF مع تخصيص التصيير
            workbook.Save("DrawObjectEventHandlerDemo.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // عرض معالجة أنواع كائنات التصيير المختلفة
            switch (drawObject.Type)
            {
                case DrawObjectEnum.Cell:
                    Console.WriteLine($"Rendering cell at ({x}, {y})");
                    break;
                    
                case DrawObjectEnum.Image:
                    Console.WriteLine($"Rendering image at ({x}, {y})");
                    break;
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


