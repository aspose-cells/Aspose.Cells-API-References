---
title: "فئة DrawObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Rendering.DrawObject. سيتم تهيئة DrawObject وإرجاعه أثناء التصيير"
type: docs
url: /ar/net/aspose.cells.rendering/drawobject/
---
## DrawObject class

سيتم تهيئة DrawObject وإرجاعه عند التصيير.

```csharp
public class DrawObject
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Cell](../../aspose.cells.rendering/drawobject/cell/) { get; } | يشير إلى كائن Cell أثناء التصيير. يمكن الوصول إلى جميع خصائص الخلية. |
| [CurrentPage](../../aspose.cells.rendering/drawobject/currentpage/) { get; } | يشير إلى فهرس الصفحة لكائن DrawObject. فهرس الصفحة يبدأ من الصفر. تحتوي ورقة واحدة على عدة صفحات أثناء التصيير. |
| [ImageBytes](../../aspose.cells.rendering/drawobject/imagebytes/) { get; } | يشير إلى بايتات الصورة للمخطط أو الشكل المصدّر أثناء التصيير. |
| [Shape](../../aspose.cells.rendering/drawobject/shape/) { get; } | يشير إلى كائن Shape أثناء التصيير. يمكن الوصول إلى جميع خصائص الشكل. |
| [SheetIndex](../../aspose.cells.rendering/drawobject/sheetindex/) { get; } | يشير إلى فهرس الورقة الحالية لكائن DrawObject. |
| [TotalPages](../../aspose.cells.rendering/drawobject/totalpages/) { get; } | يشير إلى إجمالي الصفحات في التصيير الحالي. |
| [Type](../../aspose.cells.rendering/drawobject/type/) { get; } | يشير إلى نوع DrawObject. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;

namespace AsposeCellsExamples
{
    // تنفيذ مخصص لـ DrawObjectEventHandler
    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"Drawing object at X: {x}, Y: {y}, Width: {width}, Height: {height}");
            Console.WriteLine($"Object Type: {drawObject.Type}");
            Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}");

            if (drawObject.Cell != null)
            {
                Console.WriteLine($"Rendering Cell: {drawObject.Cell.Name}, Value: {drawObject.Cell.Value}");
            }

            if (drawObject.Shape != null)
            {
                Console.WriteLine($"Rendering Shape: {drawObject.Shape.Name}");
            }
        }
    }

    public class DrawObjectDemo
    {
        public static void RunDemo()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

            // إضافة شكل
            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddShape(Aspose.Cells.Drawing.MsoDrawingType.Rectangle, 5, 0, 5, 0, 100, 100);
            shape.Text = "Sample Shape";

            // إنشاء مثال من CustomDrawObjectEventHandler
            CustomDrawObjectEventHandler drawObjectEventHandler = new CustomDrawObjectEventHandler();

            // تعيين خيارات الصورة أو الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                DrawObjectEventHandler = drawObjectEventHandler,
                OnePagePerSheet = true,
                ImageType = Aspose.Cells.Drawing.ImageType.Png
            };

            // تصيير الورقة إلى صورة
            SheetRender sr = new SheetRender(sheet, options);
            sr.ToImage(0, "DrawObjectDemo.png");

            // احفظ المصنف
            workbook.Save("DrawObjectDemo.xlsx");
            workbook.Save("DrawObjectDemo.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


