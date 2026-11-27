---
title: "Validation.Areas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation‑egenskap. Hämtar alla CellArea som innehåller datavalideringsinställningarna"
type: docs
url: /sv/net/aspose.cells/validation/areas/
---
## Validation.Areas property

Hämtar alla [`CellArea`](../../cellarea/) som innehåller datavalideringsinställningarna.

```csharp
public CellArea[] Areas { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("Areas & rent");

            // Skapa validering för kolumn A
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "100";

            // Lägg till valideringsområden på olika rader
            validation.AddArea(new CellArea { StartRow = 46, StartColumn = 0, EndRow = 50, EndColumn = 0 });
            validation.AddArea(new CellArea { StartRow = 92, StartColumn = 0, EndRow = 96, EndColumn = 0 });
            validation.AddArea(new CellArea { StartRow = 138, StartColumn = 0, EndRow = 142, EndColumn = 0 });

            // Demonstrera åtkomst till valideringsområden
            CellArea area1 = (CellArea)validation.Areas[0];
            Console.WriteLine($"Area 1 StartRow: {area1.StartRow}"); // Output: 46
            
            CellArea area2 = (CellArea)validation.Areas[1];
            Console.WriteLine($"Area 2 StartRow: {area2.StartRow}"); // Output: 92
            
            CellArea area3 = (CellArea)validation.Areas[2];
            Console.WriteLine($"Area 3 StartRow: {area3.StartRow}"); // Output: 138
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


