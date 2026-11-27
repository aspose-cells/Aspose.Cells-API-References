---
title: "ValidationCollection.GetValidationInCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ValidationCollection-metoden. Hämtar valideringen som tillämpas på den angivna cellen"
type: docs
url: /sv/net/aspose.cells/validationcollection/getvalidationincell/
---
## ValidationCollection.GetValidationInCell method

Hämtar valideringen som tillämpas på den angivna cellen.

```csharp
public Validation GetValidationInCell(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |

### Returvärde

Returnerar ett [`Validation`](../../validation/)‑objekt eller null om det inte finns någon validering för den angivna cellen

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodGetValidationInCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till datavalidering i cell A1 (0,0)
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "\"Option1,Option2,Option3\"";
            
            // Skapa CellArea med StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Hämta validering från cell A1 (0,0)
            Validation validationInCell = worksheet.Validations.GetValidationInCell(0, 0);
            
            if (validationInCell != null && validationInCell.Type == ValidationType.List)
            {
                Console.WriteLine("Cell A1 has list validation with formula: " + validationInCell.Formula1);
            }
        }
    }
}
```

### Se även

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


