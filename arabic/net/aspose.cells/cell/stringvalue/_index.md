---
title: "Cell.StringValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تحصل على القيمة النصية الموجودة في الخلية. إذا كان نوع هذه الخلية هو نص فستُرجع القيمة النصية نفسها. بالنسبة لأنواع الخلايا الأخرى سيتم إرجاع القيمة النصية المُنسقة وفق النمط المحدد لهذه الخلية. القيمة النصية المُنسقة للخلية هي نفسها ما يمكنك الحصول عليه من Excel عند نسخ الخلية كنص مثل نسخ الخلية إلى محرر نصوص أو تصدير إلى CSV"
type: docs
url: /ar/net/aspose.cells/cell/stringvalue/
---
## Cell.StringValue property

يحصل على القيمة النصية الموجودة في الخلية. إذا كان نوع هذه الخلية هو نص، فسيتم إرجاع القيمة النصية نفسها. بالنسبة لأنواع الخلايا الأخرى، سيتم إرجاع القيمة النصية المُنسقة (المُنسقة باستخدام النمط المحدد لهذه الخلية). القيمة النصية المُنسقة للخلية هي نفسها ما يمكنك الحصول عليه من Excel عند نسخ خلية كنص (مثل نسخ الخلية إلى محرر نصوص أو تصدير إلى CSV).

```csharp
public string StringValue { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyStringValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين بعض القيم
            cells["A1"].PutValue("Hello");
            cells["A2"].PutValue(123);
            cells["A3"].PutValue(DateTime.Now);
            cells["A4"].Formula = "=A1&A2";

            // حساب الصيغ
            workbook.CalculateFormula();

            // عرض خاصية StringValue
            Console.WriteLine("A1 StringValue: " + cells["A1"].StringValue);
            Console.WriteLine("A2 StringValue: " + cells["A2"].StringValue);
            Console.WriteLine("A3 StringValue: " + cells["A3"].StringValue);
            Console.WriteLine("A4 StringValue: " + cells["A4"].StringValue);

            // إظهار حالة قيمة الخطأ
            Cell errorCell = cells["B1"];
            errorCell.Formula = "=1/0";
            workbook.CalculateFormula();
            Console.WriteLine("B1 (Error) StringValue: " + errorCell.StringValue);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


