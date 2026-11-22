---
title: "ExportRangeToJsonOptions.Indent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportRangeToJsonOptions. تشير إلى المسافة البادئة"
type: docs
url: /ar/net/aspose.cells.utility/exportrangetojsonoptions/indent/
---
## ExportRangeToJsonOptions.Indent property

يشير إلى المسافة البادئة.

```csharp
public string Indent { get; set; }
```

### ملاحظات

إذا كانت المسافة البادئة فارغة أو null، فإن JSON المُصدَّر غير مُنسق.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء مثال ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // عرض المسافة البادئة الحالية (الافتراضي هو null)
            Console.WriteLine("Current Indent value: " + (options.Indent ?? "null"));

            // تصدير بالمسافة البادئة الافتراضية (JSON مضغوط)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");
            string jsonWithoutIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without indent:\n" + jsonWithoutIndent);

            // ضبط المسافة البادئة إلى 4 مسافات
            options.Indent = "    ";
            string jsonWithIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("\nJSON with 4-space indent:\n" + jsonWithIndent);

            // ضبط المسافة البادئة إلى حرف الجدولة
            options.Indent = "\t";
            string jsonWithTabIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("\nJSON with tab indent:\n" + jsonWithTabIndent);
        }
    }
}
```

### انظر أيضًا

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


