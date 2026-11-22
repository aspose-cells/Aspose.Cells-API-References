---
title: "ImageOrPrintOptions.GridlineColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. يحصل أو يضبط لون خط الشبكة"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

يحصل أو يضبط gridline colr.

```csharp
public Color GridlineColor { get; set; }
```

### ملاحظات

سيتجاهل إعدادات لون خطوط الشبكة في الملف المصدر.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية حتى يحتوي ورقة العمل على محتوى
            worksheet.Cells["A1"].PutValue("Demo for GridlineColor property");

            try
            {
                // إنشاء نسخة من ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // اعرض قيمة GridlineColor الحالية (للقراءة فقط أو للقراءة/الكتابة)
                // يفترض أن نوع الخاصية هو System.Drawing.Color
                Console.WriteLine("Current GridlineColor: " + options.GridlineColor);

                // يمكنك اختيارياً تحويل الورقة إلى صورة لرؤية تأثير لون خط الشبكة الافتراضي
                // (لا حاجة لتغيير القيمة؛ نحن فقط نوضح الاستخدام.)
                SheetRender renderer = new SheetRender(worksheet, options);
                renderer.ToImage(0, "GridlineColorDemo.png");

                // احفظ دفتر العمل (اختياري)
                workbook.Save("GridlineColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


