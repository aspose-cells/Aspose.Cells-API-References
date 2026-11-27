---
title: "Validation.RemoveACell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsmetod. Ta bort valideringsinställningarna i cellen"
type: docs
url: /sv/net/aspose.cells/validation/removeacell/
---
## Validation.RemoveACell method

Ta bort valideringsinställningarna i cellen.

```csharp
public void RemoveACell(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till datavalidering till den första cellen
            Validation validation = worksheet.Validations[0];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.Type = ValidationType.List;
            validation.Formula1 = "1,2,3";
            
            // Lägg till en annan cell till valideringen
            validation.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 1, EndColumn = 1 });
            
            // Ta bort den andra cellen från valideringen
            validation.RemoveACell(1, 1);
            
            Console.WriteLine("Cell removed from validation successfully.");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


