---
title: "PaginatedSaveOptions.GridlineColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تحصل أو تعين لون خطوط الشبكة"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

يحصل أو يضبط لون خطوط الشبكة.

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
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Gridline Color Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // أنشئ خيارات حفظ PDF
                PdfSaveOptions options = new PdfSaveOptions();

                // اعرض قيمة GridlineColor الافتراضية
                Console.WriteLine("Default GridlineColor: " + options.GridlineColor);

                // حدد لون خطوط شبكة جديد
                options.GridlineColor = Color.Red;

                // اعرض قيمة GridlineColor المحدثة
                Console.WriteLine("Updated GridlineColor: " + options.GridlineColor);

                // احفظ المصنف مع إعداد لون خطوط الشبكة
                workbook.Save("GridlineColorDemo.pdf", options);

                Console.WriteLine("PDF saved with custom gridline color.");
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

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


