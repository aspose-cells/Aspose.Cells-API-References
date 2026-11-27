---
title: "ValidationCollection.RemoveACell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ValidationCollection-metod. Tar bort alla valideringsinställningar på cellen"
type: docs
url: /sv/net/aspose.cells/validationcollection/removeacell/
---
## ValidationCollection.RemoveACell method

Tar bort alla valideringsinställningar på cellen.

```csharp
public void RemoveACell(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex för cellen. |
| column | Int32 | Kolumnindex för cellen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till validering i cell A1 (rad 0, kolumn 0)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Item1,Item2,Item3";

            // Ta bort validering från cell A1
            worksheet.Validations.RemoveACell(0, 0);

            Console.WriteLine("Validations count after removal: " + worksheet.Validations.Count);
        }
    }
}
```

### Se även

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


