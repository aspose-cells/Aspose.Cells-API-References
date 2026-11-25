---
title: "FormulaParseOptions.LocaleDependent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaParseOptions. Indica se la formula è formattata secondo la locale. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/formulaparseoptions/localedependent/
---
## FormulaParseOptions.LocaleDependent property

Indica se la formula è formattata per la lingua locale. Il valore predefinito è false.

```csharp
public bool LocaleDependent { get; set; }
```

### Esempi

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

### Vedi anche

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


