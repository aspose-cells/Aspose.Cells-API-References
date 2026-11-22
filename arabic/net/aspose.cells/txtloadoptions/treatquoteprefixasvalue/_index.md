---
title: "TxtLoadOptions.TreatQuotePrefixAsValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. تشير إلى ما إذا كان يجب اعتبار علامة الاقتباس المفردة الأولية جزءًا من قيمة الخلية. القيمة الافتراضية هي true. إذا كانت false سيتم إزالة علامة الاقتباس المفردة الأولية من قيمة الخلايا المقابلة وسيتم تعيين QuotePrefix إلى true للخلية."
type: docs
url: /ar/net/aspose.cells/txtloadoptions/treatquoteprefixasvalue/
---
## TxtLoadOptions.TreatQuotePrefixAsValue property

تشير إلى ما إذا كان يجب اعتبار علامة الاقتباس المفردة الأولية جزءًا من قيمة الخلية. القيمة الافتراضية هي true. إذا كانت false، سيتم إزالة علامة الاقتباس المفردة الأولية من قيمة الخلية المقابلة وسيتم تعيين [`QuotePrefix`](../../style/quoteprefix/) إلى true للخلية.

```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTreatQuotePrefixAsValueDemo
    {
        public static void Run()
        {
            // إنشاء بيانات CSV عينة مع بادئات الاقتباس
            string csvData = "ID,Name,Value\n1,\"'Apple\",100\n2,\"'Orange\",200";
            string filePath = "test.csv";

            // حفظ بيانات CSV في ملف
            File.WriteAllText(filePath, csvData);

            // السيناريو 1: TreatQuotePrefixAsValue = false (الافتراضي)
            var loadOptions1 = new TxtLoadOptions();
            loadOptions1.TreatQuotePrefixAsValue = false;
            
            var workbook1 = new Workbook(filePath, loadOptions1);
            var worksheet1 = workbook1.Worksheets[0];
            Console.WriteLine("TreatQuotePrefixAsValue = false:");
            Console.WriteLine("Cell B2 value: " + worksheet1.Cells["B2"].Value); // Will show 'Apple (quote treated as formatting)

            // السيناريو 2: TreatQuotePrefixAsValue = true
            var loadOptions2 = new TxtLoadOptions();
            loadOptions2.TreatQuotePrefixAsValue = true;
            
            var workbook2 = new Workbook(filePath, loadOptions2);
            var worksheet2 = workbook2.Worksheets[0];
            Console.WriteLine("\nTreatQuotePrefixAsValue = true:");
            Console.WriteLine("Cell B2 value: " + worksheet2.Cells["B2"].Value); // Will show 'Apple (quote treated as value)

            // تنظيف
            File.Delete(filePath);
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


