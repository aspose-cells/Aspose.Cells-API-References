---
title: "Cell.Formula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تحصل على صيغة الخلية أو تعيينها"
type: docs
url: /ar/net/aspose.cells/cell/formula/
---
## Cell.Formula property

تحصل على صيغة الخلية أو تعيينها من خلال [`Cell`](../).

```csharp
public string Formula { get; set; }
```

### ملاحظات

دائمًا ما يبدأ نص الصيغة بعلامة مساواة (=). ويرجى دائمًا استخدام الفاصلة (,) كفاصل للمعاملات، مثل "=SUM(A1, E1, H2)".

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // حدد القيم في الخلايا التي ستُستخدم في الصيغة
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A1"].PutValue(100);

            // حدد الصيغة في الخلية B6
            worksheet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + A1";

            // احسب الصيغة
            workbook.CalculateFormula();

            // اعرض النتيجة
            Console.WriteLine("Formula result in B6: " + worksheet.Cells["B6"].Value);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


