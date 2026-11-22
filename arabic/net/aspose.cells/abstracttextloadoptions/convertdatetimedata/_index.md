---
title: "AbstractTextLoadOptions.ConvertDateTimeData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractTextLoadOptions. الحصول على أو تعيين قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات تاريخ. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات تاريخ. القيمة الافتراضية هي true.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertDateTimeDataDemo
    {
        public static void Run()
        {
            // إنشاء بيانات CSV مع سلسلة تاريخ
            string csvData = "\"2023-05-15\",\"123.45\"";

            // إنشاء خيارات تحميل النص مع تعيين ConvertDateTimeData إلى false
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            options.ConvertDateTimeData = false;
            options.ConvertNumericData = false;

            // تحميل بيانات CSV
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // إخراج القيم (يجب أن تظل كسلاسل)
            Console.WriteLine("Cell A1 value: " + worksheet.Cells[0, 0].StringValue); // Outputs "2023-05-15" as string
            Console.WriteLine("Cell B1 value: " + worksheet.Cells[0, 1].StringValue); // Outputs "123.45" as string

            // الآن قم بالتحميل مع تعيين ConvertDateTimeData إلى true
            options.ConvertDateTimeData = true;
            options.ConvertNumericData = true;
            workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            worksheet = workbook.Worksheets[0];

            // إخراج القيم المحوّلة
            Console.WriteLine("Cell A1 value (converted): " + worksheet.Cells[0, 0].DateTimeValue); // Outputs DateTime
            Console.WriteLine("Cell B1 value (converted): " + worksheet.Cells[0, 1].DoubleValue);  // Outputs 123.45 as double
        }
    }
}
```

### انظر أيضًا

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


