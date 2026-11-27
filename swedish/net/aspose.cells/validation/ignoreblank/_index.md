---
title: "Validation.IgnoreBlank"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsegenskap. Anger om tomma värden är tillåtna av områdesdatavalideringen"
type: docs
url: /sv/net/aspose.cells/validation/ignoreblank/
---
## Validation.IgnoreBlank property

Indikerar om tomma värden är tillåtna av data validation för intervallet.

```csharp
public bool IgnoreBlank { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyIgnoreBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            ValidationCollection validations = sheet.Validations;
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 1;
            area.StartColumn = 0;
            area.EndColumn = 1;
            Validation validation = validations[validations.Add(area)];

            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "2";
            validation.Formula2 = "20";
            validation.IgnoreBlank = true;

            Console.WriteLine("Validation created with IgnoreBlank set to: " + validation.IgnoreBlank);
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


