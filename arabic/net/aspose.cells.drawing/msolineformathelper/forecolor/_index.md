---
title: "MsoLineFormatHelper.ForeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoLineFormatHelper. تحصل وتعيّن لون الخط الأمامي للحد"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformathelper/forecolor/
---
## MsoLineFormatHelper.ForeColor property

يحصل على ويضبط لون مقدمة خط الحدود.

```csharp
public Color ForeColor { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyForeColorDemo
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

                // اعرض قيمة ForeColor الحالية
                Console.WriteLine("Current ForeColor: " + lineFormat.ForeColor);

                // عيّن ForeColor جديد (لأنها قراءة/كتابة)
                lineFormat.ForeColor = Color.Red;
                Console.WriteLine("Updated ForeColor: " + lineFormat.ForeColor);

                // إظهار كيف تؤثر الخاصية على السلوك
                Console.WriteLine("Line fore color has been updated to: " + lineFormat.ForeColor);

                // حفظ النتيجة
                workbook.Save("ForeColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line fore color.");
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


