---
title: "TxtLoadOptions.HasFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. تشير إلى ما إذا كان النص صيغة إذا بدأ بـ"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/hasformula/
---
## TxtLoadOptions.HasFormula property

يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=".

```csharp
public bool HasFormula { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل النص وتمكين تحليل الصيغ
            TxtLoadOptions options = new TxtLoadOptions();
            options.HasFormula = true;
            options.SeparatorString = "|";

            // تحميل دفتر عمل مع صيغ في ملف النص
            Workbook workbook = new Workbook("example.csv", options);
            
            // الوصول إلى خلية تحتوي على صيغة وعرضها
            Console.WriteLine("Cell K2 formula: " + workbook.Worksheets[0].Cells["K2"].Formula);
            
            // احفظ المصنف
            workbook.Save("example_output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


