---
title: "DrawObject.CurrentPage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DrawObject. تشير إلى فهرس الصفحة لكائن DrawObject. فهرس الصفحة يبدأ من الصفر. تحتوي ورقة واحدة على عدة صفحات عند التصيير"
type: docs
url: /ar/net/aspose.cells.rendering/drawobject/currentpage/
---
## DrawObject.CurrentPage property

يشير إلى فهرس الصفحة لكائن DrawObject. فهرس الصفحة يبدأ من الصفر. تحتوي ورقة واحدة على عدة صفحات أثناء التصيير.

```csharp
public int CurrentPage { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyCurrentPageDemo
    {
        // معالج مخصص لقراءة وعرض خاصية CurrentPage
        private class CurrentPageHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // عرض قيمة خاصية CurrentPage
                Console.WriteLine($"CurrentPage: {drawObject.CurrentPage}");
                Console.WriteLine($"TotalPages: {drawObject.TotalPages}");
                Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // إنشاء مصنف جديد والوصول إلى ورقة العمل الأولى
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف بعض البيانات العينية لجعل التصيير ذا معنى
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["A2"].PutValue("More Data");
                worksheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // أضف شكلاً لتوليد كائنات رسم من نوع الشكل
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // قم بإعداد خيارات التصيير باستخدام معالج الرسم المخصص لدينا
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CurrentPageHandler()
                };

                // قم بتجسيد ورقة العمل لتفعيل أحداث DrawObject
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "CurrentPageDemo.png");

                // احفظ المصنف
                workbook.Save("CurrentPageDemo.xlsx");
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


