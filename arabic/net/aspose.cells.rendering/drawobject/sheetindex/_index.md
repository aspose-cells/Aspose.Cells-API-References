---
title: "DrawObject.SheetIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DrawObject. تشير إلى فهرس الورقة الحالي لـ DrawObject"
type: docs
url: /ar/net/aspose.cells.rendering/drawobject/sheetindex/
---
## DrawObject.SheetIndex property

يشير إلى فهرس الورقة الحالية لكائن DrawObject.

```csharp
public int SheetIndex { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    // معالج مخصص يقرأ ويعرض SheetIndex لكل DrawObject
    class SheetIndexReaderHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
            Console.WriteLine($"Page: {drawObject.CurrentPage + 1}/{drawObject.TotalPages}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");
            Console.WriteLine();
        }
    }

    public class DrawObjectPropertySheetIndexDemo
    {
        public static void Run()
        {
            try
            {
                // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // املأ بعض الخلايا بمحتوى للعرض
                sheet.Cells["A1"].PutValue("First");
                sheet.Cells["A2"].PutValue("Second");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // أضف شكلاً بحيث يتم إنشاء كائنات رسم الشكل أيضًا
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // قم بإعداد خيارات التصيير باستخدام معالجنا المخصص
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new SheetIndexReaderHandler()
                };

                // قم بتصيير ورقة العمل – هذا يُطلق أحداث DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "SheetIndexDemo.png");

                // احفظ دفتر العمل (اختياري)
                workbook.Save("SheetIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


