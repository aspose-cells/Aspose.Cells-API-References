---
title: "FormulaParseOptions.LocaleDependent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaParseOptions. Indica si la fórmula está formateada según la configuración regional. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/formulaparseoptions/localedependent/
---
## FormulaParseOptions.LocaleDependent property

Indica si la fórmula está formateada según la configuración regional. El valor predeterminado es false.

```csharp
public bool LocaleDependent { get; set; }
```

### Ejemplos

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

### Ver también

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


