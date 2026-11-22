---
title: "DrawObject.Shape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DrawObject. تشير إلى كائن Shape عند التصيير. يمكن الوصول إلى جميع خصائص الشكل"
type: docs
url: /ar/net/aspose.cells.rendering/drawobject/shape/
---
## DrawObject.Shape property

يشير إلى كائن Shape أثناء التصيير. يمكن الوصول إلى جميع خصائص الشكل.

```csharp
public Shape Shape { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyShapeDemo
    {
        public static void Run()
        {
            try
            {
                // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف بيانات عينة لجعل التصيير ذا معنى
                worksheet.Cells["A1"].Value = "Sample Data";
                worksheet.Cells["A2"].Value = "More Data";

                // إضافة شكل إلى ورقة العمل
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // قم بإعداد خيارات التصيير باستخدام معالج مخصص
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new ShapePropertyHandler()
                };

                // قم بتصيير ورقة العمل - سيؤدي ذلك إلى تشغيل أحداث DrawObject
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "ShapeDemo.png");

                // احفظ المصنف
                workbook.Save("ShapeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // معالج مخصص لالتقاط أحداث DrawObject وقراءة خاصية Shape
        private class ShapePropertyHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                if (drawObject.Shape != null)
                {
                    Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                    Console.WriteLine($"Shape Name: {drawObject.Shape.Name}");
                    Console.WriteLine($"Shape Text: {drawObject.Shape.Text}");
                    Console.WriteLine($"Shape Width: {drawObject.Shape.Width} pixels");
                    Console.WriteLine($"Shape Height: {drawObject.Shape.Height} pixels");
                    Console.WriteLine($"Shape Type: {drawObject.Shape.AutoShapeType}");
                    Console.WriteLine();
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../../aspose.cells.drawing/shape/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


