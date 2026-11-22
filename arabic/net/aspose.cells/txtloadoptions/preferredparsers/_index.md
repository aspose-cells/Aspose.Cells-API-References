---
title: "TxtLoadOptions.PreferredParsers"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. تحصل وتضبط محللات القيم المفضلة لتحميل ملف نصي"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/preferredparsers/
---
## TxtLoadOptions.PreferredParsers property

يحصل على ويضبط محللات القيم المفضلة لتحميل ملف نصي.

```csharp
public ICustomParser[] PreferredParsers { get; set; }
```

### ملاحظات

parsers[0] هو المحلل الذي سيُستخدم للعمود الأول في ملف قالب النص، parsers[1] هو المحلل الذي سيُستخدم للعمود الثاني، ...إلخ. الأخير (parsers[parsers.length-1]) سيُستخدم لجميع الأعمدة الأخرى بدءًا من parsers.length-1. إذا كان أحد العناصر null، سيتم تحليل العمود المقابل بواسطة المحلل الافتراضي لـ Aspose.Cells.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyPreferredParsersDemo
    {
        private class StringParser : ICustomParser
        {
            public bool Parse(string value, out object result)
            {
                result = value; // Always return as string
                return true;
            }

            public object ParseObject(string value)
            {
                return value; // Always return as string
            }

            public string GetFormat()
            {
                return "String"; // Return format description
            }
        }

        public static void Run()
        {
            // إنشاء خيارات تحميل CSV
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            
            // تعيين المحللات المفضلة - أولاً جرب محلل السلسلة المخصص، ثم المحللات الافتراضية
            options.PreferredParsers = new ICustomParser[] { new StringParser(), null };

            // بيانات CSV عينة مع تواريخ
            string csvData = "\"2018-10-08\",2018-10-08\n\"2018-10-08\",2018-10-08";
            
            // تحميل دفتر العمل مع الخيارات
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Cells cells = workbook.Worksheets[0].Cells;

            // تحقق من نتائج التحليل
            Console.WriteLine("A1 Type: " + cells[0, 0].Type); // Should be string
            Console.WriteLine("A1 Value: " + cells[0, 0].StringValue); // "2018-10-08"
            Console.WriteLine("B1 Type: " + cells[0, 1].Type); // Should be DateTime
            Console.WriteLine("B1 Value: " + cells[0, 1].DateTimeValue); // 10/8/2018
        }
    }
}
```

### انظر أيضًا

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


