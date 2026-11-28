---
title: "FormulaParseOptions.LocaleDependent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaParseOptions özelliği. Formülün yerel ayarlara göre biçimlendirilip biçimlendirilmediğini belirler. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/formulaparseoptions/localedependent/
---
## FormulaParseOptions.LocaleDependent property

Formülün yerel formatta olup olmadığı. Varsayılan değer false'tur.

```csharp
public bool LocaleDependent { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


