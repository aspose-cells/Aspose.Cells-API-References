---
title: "FormulaParseOptions.LocaleDependent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaParseOptions. ما إذا كانت الصيغة مهيأة حسب الإعدادات الإقليمية. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/formulaparseoptions/localedependent/
---
## FormulaParseOptions.LocaleDependent property

ما إذا كانت الصيغة مُنسقة حسب اللغة المحلية. القيمة الافتراضية هي false.

```csharp
public bool LocaleDependent { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyLocaleDependentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            FormulaParseOptions options = new FormulaParseOptions
            {
                LocaleDependent = true,
                R1C1Style = false
            };

            worksheet.Cells["A1"].SetFormula("=TEXT(TODAY(),\"[$-fr-FR]dddd, dd mmmm yyyy\")", options);
            
            workbook.Save("LocaleDependentFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


