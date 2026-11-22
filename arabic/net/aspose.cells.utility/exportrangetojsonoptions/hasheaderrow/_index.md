---
title: "ExportRangeToJsonOptions.HasHeaderRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportRangeToJsonOptions. تشير إلى ما إذا كان النطاق يحتوي على صف رأس"
type: docs
url: /ar/net/aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/
---
## ExportRangeToJsonOptions.HasHeaderRow property

يشير إلى ما إذا كان النطاق يحتوي على صف رأس.

```csharp
public bool HasHeaderRow { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء البيانات التجريبية مع رؤوس الأعمدة
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء نطاق للتصدير
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // إنشاء مثال ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();

            // عرض قيمة HasHeaderRow الحالية (القيمة الافتراضية هي false)
            Console.WriteLine("Current HasHeaderRow value: " + options.HasHeaderRow);

            // ضبط HasHeaderRow إلى true
            options.HasHeaderRow = true;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // تصدير إلى JSON مع رؤوس الأعمدة
            string jsonWithHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // ضبط HasHeaderRow إلى false
            options.HasHeaderRow = false;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // تصدير إلى JSON بدون رؤوس الأعمدة
            string jsonWithoutHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without headers:\n" + jsonWithoutHeaders);

            // احفظ المصنف
            workbook.Save("PropertyHasHeaderRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


