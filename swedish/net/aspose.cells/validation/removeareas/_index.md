---
title: "Validation.RemoveAreas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation-metod. Tar bort denna validering från angivna områden"
type: docs
url: /sv/net/aspose.cells/validation/removeareas/
---
## Validation.RemoveAreas method

Tar bort denna validering från angivna områden.

```csharp
public void RemoveAreas(CellArea[] areas)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| områden | CellArea[] | områdena där dessa valideringsinställningar ska tas bort. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodRemoveAreasWithCellAreaArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till datavalidering i kalkylbladet
            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            
            // Konfigurera valideringsinställningar
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "10";

            // Skapa två cellområden för validering
            CellArea area1 = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 1,
                EndColumn = 1
            };  // A1:B2
            CellArea area2 = new CellArea
            {
                StartRow = 2,
                StartColumn = 2,
                EndRow = 3,  // Original code had (2,2,1,1) which would be invalid endRow < startRow
                EndColumn = 3
            };  // C3:D4 (corrected end coordinates)
            
            // Lägg till områden till validering
            validation.AddArea(area1);
            validation.AddArea(area2);
            Console.WriteLine($"Added areas: {validation.Areas.Length}");

            try
            {
                // Skapa en array med ett område att ta bort
                CellArea[] removeAreas = { area1 };
                
                // Utför metoden RemoveAreas
                validation.RemoveAreas(removeAreas);
                Console.WriteLine($"Remaining areas after removal: {validation.Areas.Length}");
                
                // Visa koordinater för återstående områden
                foreach (CellArea remainingArea in validation.Areas)
                {
                    Console.WriteLine($"Area: {remainingArea.StartRow},{remainingArea.StartColumn} to {remainingArea.EndRow},{remainingArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Spara modifierad arbetsbok
            workbook.Save("ValidationRemoveAreasDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


