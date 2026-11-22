---
title: "FormulaParseOptions.R1C1Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaParseOptions. ما إذا كانت الصيغة بنمط الإشارة R1C1. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/formulaparseoptions/r1c1style/
---
## FormulaParseOptions.R1C1Style property

ما إذا كانت الصيغة بنمط الإشارة R1C1. القيمة الافتراضية هي false.

```csharp
public bool R1C1Style { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyR1C1StyleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // تعيين القيم للخلايا المشار إليها
            cells["D7"].PutValue(10);
            cells["D8"].PutValue(20);
            cells["D9"].PutValue(30);
            cells["C7"].PutValue(1);
            cells["C8"].PutValue(2);
            cells["C9"].PutValue(3);

            // تعيين صيغة مصفوفة باستخدام نمط R1C1
            cells[7, 4].SetArrayFormula("=TREND(RC[-1]:R[2]C[-1],RC[-2]:R[2]C[-2])", 3, 1,
                new FormulaParseOptions() { R1C1Style = true });

            // إخراج صيغ R1C1
            for (int i = 7; i < 10; i++)
            {
                Console.WriteLine($"Cell E{i + 1} R1C1 formula: {cells[i, 4].R1C1Formula}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


