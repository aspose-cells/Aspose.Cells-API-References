---
title: "MsoLineFormatHelper.BackColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoLineFormatHelper. يحصل ويضبط BackColor للخط الحدودي"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformathelper/backcolor/
---
## MsoLineFormatHelper.BackColor property

يحصل على ويضبط لون خلفية خط الحدود.

```csharp
public Color BackColor { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyBackColorDemo
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

                // احصل على تنسيق الخط
                MsoLineFormat lineFormat = shape.LineFormat;

                // اعرض قيمة BackColor الحالية
                Console.WriteLine("Current BackColor: " + lineFormat.BackColor);

                // عيّن قيمة BackColor جديدة (لأنها قابلة للقراءة/الكتابة)
                lineFormat.BackColor = Color.LightBlue;
                Console.WriteLine("Updated BackColor: " + lineFormat.BackColor);

                // إظهار كيف تؤثر الخاصية على السلوك
                Console.WriteLine("Line back color has been updated to: " + lineFormat.BackColor);

                // حفظ النتيجة
                workbook.Save("BackColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line back color.");
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

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


