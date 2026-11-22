---
title: "MsoLineFormatHelper.Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoLineFormatHelper. يرجع كائن Style الذي يمثل نمط النطاق المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformathelper/style/
---
## MsoLineFormatHelper.Style property

يرجع كائن Style يمثل نمط النطاق المحدد.

```csharp
public MsoLineStyle Style { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل نموذجية
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // إنشاء شكل لتوضيح تنسيق الخط
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // احصل على تنسيق الخط مباشرة (يبدو أن MsoLineFormatHelper فئة مساعدة)
                // نظرًا لعدم إمكانية إنشاء كائن MsoLineFormatHelper مباشرةً، سنعمل مع خاصية LineFormat
                MsoLineFormat lineFormat = shape.LineFormat;

                // اعرض قيمة Style الحالية
                Console.WriteLine("Current Line Style: " + lineFormat.Style);

                // عيّن نمطًا جديدًا (لأن Style قابلة للقراءة/الكتابة)
                lineFormat.Style = MsoLineStyle.ThickBetweenThin;
                Console.WriteLine("Updated Line Style: " + lineFormat.Style);

                // إظهار كيف تؤثر الخاصية على السلوك
                Console.WriteLine("Line style has been updated to: " + lineFormat.Style);

                // حفظ النتيجة
                workbook.Save("LineStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line style.");
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

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


