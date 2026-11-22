---
title: "DrawObject.Cell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DrawObject. تشير إلى كائن Cell عند التصيير. يمكن الوصول إلى جميع خصائص الخلية"
type: docs
url: /ar/net/aspose.cells.rendering/drawobject/cell/
---
## DrawObject.Cell property

يشير إلى كائن Cell أثناء التصيير. يمكن الوصول إلى جميع خصائص الخلية.

```csharp
public Cell Cell { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    // معالج مخصص لالتقاط أحداث DrawObject وقراءة خاصية Cell
    public class CellInfoDrawHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // إخراج معلومات أساسية عن كائن الرسم
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");

            // توضيح قراءة خاصية Cell للقراءة فقط
            if (drawObject.Cell != null)
            {
                var cell = drawObject.Cell;
                Console.WriteLine($"Cell Name: {cell.Name}");
                Console.WriteLine($"Cell Value: {cell.Value}");
                Console.WriteLine($"Cell Row: {cell.Row}, Column: {cell.Column}");
            }
        }
    }

    public class DrawObjectPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // أضف بعض البيانات النموذجية إلى الخلايا
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // أضف شكلاً لضمان رفع أحداث رسم الشكل أيضًا
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // قم بإعداد خيارات التصيير باستخدام معالج الرسم المخصص لدينا
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CellInfoDrawHandler()
                };

                // قم بتصيير ورقة العمل – سيؤدي ذلك إلى تشغيل أحداث DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectCellDemo.png");

                // احفظ دفتر العمل (اختياري)
                workbook.Save("DrawObjectCellDemo.xlsx");
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

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


