---
title: "Worksheet.ShowFormulas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Worksheet property. يشير إلى ما إذا كان سيتم إظهار الصيغ أو نتائجها"
type: docs
url: /ar/net/aspose.cells/worksheet/showformulas/
---
## Worksheet.ShowFormulas property

يشير إلى ما إذا كان يجب إظهار الصيغ أو نتائجها.

```csharp
public bool ShowFormulas { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShowFormulasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ضع صيغة في الخلية A1
            worksheet.Cells["A1"].Formula = "=1+2+3";
            
            // إظهار القيمة المحسوبة مبدئياً
            worksheet.ShowFormulas = false;
            Console.WriteLine("ShowFormulas OFF: " + worksheet.Cells["A1"].StringValue);

            // بدّل لإظهار نص الصيغة
            worksheet.ShowFormulas = true;
            Console.WriteLine("ShowFormulas ON: " + worksheet.Cells["A1"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


