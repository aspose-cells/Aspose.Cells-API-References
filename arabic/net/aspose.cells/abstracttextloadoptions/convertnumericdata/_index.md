---
title: "AbstractTextLoadOptions.ConvertNumericData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractTextLoadOptions. تحصل أو تعيين قيمة تشير إلى ما إذا كان النص في ملف النص يُحوَّل إلى بيانات رقمية. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات رقمية. القيمة الافتراضية هي true.

```csharp
public bool ConvertNumericData { get; set; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // إنشاء بيانات CSV نموذجية تحتوي على قيم رقمية ونصية
            string csvData = "ID,Name,Price,Quantity\n" +
                            "1,Product A,19.99,5\n" +
                            "2,Product B,\"24.50\",\"10\"\n" +
                            "3,Product C,15.75,\"N/A\"";

            // إنشاء TxtLoadOptions مع تعيين ConvertNumericData إلى true
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv)
            {
                ConvertNumericData = true,
                ConvertDateTimeData = true
            };

            // حمّل بيانات CSV إلى دفتر عمل
            Workbook workbook = new Workbook(new System.IO.MemoryStream(Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // إظهار التحويل الرقمي
            Console.WriteLine("Cell B2 (Product A Price) value type: " + worksheet.Cells["B2"].Value.GetType());
            Console.WriteLine("Cell B2 value: " + worksheet.Cells["B2"].Value);

            // إظهار القيم النصية التي لا يمكن تحويلها
            Console.WriteLine("\nCell D4 (N/A) value type: " + worksheet.Cells["D4"].Value.GetType());
            Console.WriteLine("Cell D4 value: " + worksheet.Cells["D4"].Value);

            // إظهار كيف يتم تحويل الأرقام المقتبسة حتى عندما يكون ConvertNumericData true
            Console.WriteLine("\nCell C3 (Quoted \"24.50\") value type: " + worksheet.Cells["C3"].Value.GetType());
            Console.WriteLine("Cell C3 value: " + worksheet.Cells["C3"].Value);
        }
    }
}
```

### انظر أيضًا

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


