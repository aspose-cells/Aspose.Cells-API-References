---
title: "ExportRangeToJsonOptions.ExportAsString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportRangeToJsonOptions. تصدر القيمة النصية للخلايا إلى json"
type: docs
url: /ar/net/aspose.cells.utility/exportrangetojsonoptions/exportasstring/
---
## ExportRangeToJsonOptions.ExportAsString property

يصدّر القيم النصية للخلايا إلى JSON.

```csharp
public bool ExportAsString { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء الخلايا بأنواع بيانات مختلفة
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("String");
            worksheet.Cells["B2"].PutValue("Hello");
            worksheet.Cells["A3"].PutValue("Number");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["B4"].PutValue(DateTime.Now);

            // إنشاء مثال ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // عرض قيمة ExportAsString الحالية
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // تصدير بدون ExportAsString (السلوك الافتراضي)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B4");
            string jsonWithoutString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without ExportAsString:\n" + jsonWithoutString);

            // ضبط ExportAsString إلى true
            options.ExportAsString = true;

            // تصدير مع ExportAsString
            string jsonWithString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with ExportAsString:\n" + jsonWithString);

            // احفظ المصنف
            workbook.Save("ExportAsStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


