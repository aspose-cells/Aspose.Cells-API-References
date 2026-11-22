---
title: "MsoLineFormatHelper.DashStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoLineFormatHelper. يحصل أو يضبط DashStyle للخط المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformathelper/dashstyle/
---
## MsoLineFormatHelper.DashStyle property

يحصل على أو يضبط نمط الشرط للخط المحدد.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyDashStyleDemo
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

                // اعرض قيمة DashStyle الحالية
                Console.WriteLine("Current DashStyle: " + lineFormat.DashStyle);

                // عيّن قيمة DashStyle جديدة (لأنها قابلة للقراءة/الكتابة)
                lineFormat.DashStyle = MsoLineDashStyle.DashDot;
                Console.WriteLine("Updated DashStyle: " + lineFormat.DashStyle);

                // إظهار كيف تؤثر الخاصية على السلوك
                Console.WriteLine("Line dash style has been updated to: " + lineFormat.DashStyle);

                // حفظ النتيجة
                workbook.Save("DashStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line dash style.");
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

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


