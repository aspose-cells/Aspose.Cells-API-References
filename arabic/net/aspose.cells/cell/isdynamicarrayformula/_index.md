---
title: "Cell.IsDynamicArrayFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخلية. تشير إلى ما إذا كانت صيغة الخلية مصفوفة ديناميكية (true) أو مصفوفة تقليدية (false)"
type: docs
url: /ar/net/aspose.cells/cell/isdynamicarrayformula/
---
## Cell.IsDynamicArrayFormula property

يشير إلى ما إذا كانت صيغة الخلية هي صيغة مصفوفة ديناميكية (true) أو صيغة مصفوفة قديمة (false).

```csharp
public bool IsDynamicArrayFormula { get; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين صيغة مصفوفة ديناميكية في الخلية A1
            worksheet.Cells["A1"].SetDynamicArrayFormula("=B1:B3", new FormulaParseOptions(), false);
            
            // التحقق مما إذا كانت الخلية تحتوي على صيغة مصفوفة ديناميكية
            Console.WriteLine("Is A1 a dynamic array formula? " + worksheet.Cells["A1"].IsDynamicArrayFormula);

            // احفظ المصنف
            string outputPath = "DynamicArrayFormulaDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with dynamic array formula at: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


