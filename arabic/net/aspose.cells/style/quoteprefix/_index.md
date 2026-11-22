---
title: "Style.QuotePrefix"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة"
type: docs
url: /ar/net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة.

```csharp
public bool QuotePrefix { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية B10 وتعيين قيمتها
            Cell cell = worksheet.Cells["B10"];
            cell.PutValue("'12345"); // Note the single quote prefix

            // احصل على نمط الخلية وقم بتمكين QuotePrefix
            Style style = cell.GetStyle();
            style.QuotePrefix = true;
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("output.xlsx");

            // تحقق من خاصية QuotePrefix
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cell loadedCell = loadedWorkbook.Worksheets[0].Cells["B10"];
            Console.WriteLine("QuotePrefix is set: " + loadedCell.GetStyle().QuotePrefix);
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


