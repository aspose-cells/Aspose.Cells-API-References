---
title: "FormulaParseOptions.LocaleDependent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaParseOptions. Indique si la formule est formatée selon la locale. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/formulaparseoptions/localedependent/
---
## FormulaParseOptions.LocaleDependent property

Indique si la formule est formatée selon la locale. La valeur par défaut est false.

```csharp
public bool LocaleDependent { get; set; }
```

### Exemples

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

### Voir aussi

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


