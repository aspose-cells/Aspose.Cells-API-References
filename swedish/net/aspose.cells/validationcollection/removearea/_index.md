---
title: "ValidationCollection.RemoveArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ValidationCollection-metod. Tar bort alla valideringsinställningar på området"
type: docs
url: /sv/net/aspose.cells/validationcollection/removearea/
---
## ValidationCollection.RemoveArea method

Tar bort alla valideringsinställningar på området..

```csharp
public void RemoveArea(CellArea ca)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | Området som innehåller valideringsinställningarna. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionMethodRemoveAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en validering i ett specifikt område
            ValidationCollection validations = worksheet.Validations;
            CellArea validationArea = CellArea.CreateCellArea(0, 0, 5, 5);
            int validationIndex = validations.Add(validationArea);
            
            // Skapa ett område att ta bort från valideringen
            CellArea removeArea = CellArea.CreateCellArea(2, 2, 4, 4);
            
            try
            {
                // Anropa RemoveArea-metoden med CellArea-parameter
                validations.RemoveArea(removeArea);
                
                Console.WriteLine("Validation area removed successfully.");
                
                // Visa de återstående valideringsområdena
                foreach (Validation validation in validations)
                {
                    if (validation.Areas.Length > 0)
                    {
                        Console.WriteLine($"Remaining validation area: {validation.Areas[0]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("ValidationRemoveAreaDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


