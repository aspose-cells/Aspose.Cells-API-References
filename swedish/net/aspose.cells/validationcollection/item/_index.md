---
title: "ValidationCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ValidationCollection-egenskap. Hämtar Validation-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/validationcollection/item/
---
## ValidationCollection indexer

Hämtar [`Validation`](../../validation/) elementet på det angivna indexet.

```csharp
public Validation this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till datavalidering i celler
            ValidationCollection validations = sheet.Validations;
            
            // Första valideringsområdet
            Validation validation1 = validations[validations.Add()];
            validation1.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 3 });
            
            // Andra valideringsområdet
            Validation validation2 = validations[validations.Add()];
            validation2.AddArea(new CellArea { StartRow = 6, StartColumn = 1, EndRow = 6, EndColumn = 3 });

            // Åtkomst till validering med Item-egenskapen
            Validation firstValidation = validations[0];
            Console.WriteLine($"First validation has {firstValidation.Areas.Length} area(s)");

            // Verifiera områden
            foreach (CellArea area in firstValidation.Areas)
            {
                Console.WriteLine($"Area: {area.StartRow},{area.StartColumn} to {area.EndRow},{area.EndColumn}");
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


