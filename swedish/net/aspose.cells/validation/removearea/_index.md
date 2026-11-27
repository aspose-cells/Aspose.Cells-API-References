---
title: "Validation.RemoveArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsmetod. Ta bort valideringsinställningarna i intervallet"
type: docs
url: /sv/net/aspose.cells/validation/removearea/
---
## Validation.RemoveArea method

Ta bort valideringsinställningarna i området.

```csharp
public void RemoveArea(CellArea cellArea)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | CellArea | områdena där dessa valideringsinställningar ska tas bort. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en validering i kalkylbladet
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Lägg till initialt valideringsområde
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            validation.AddArea(initialArea);

            // Lägg till ett annat område till valideringen
            CellArea additionalArea = CellArea.CreateCellArea(1, 1, 1, 1);
            validation.AddArea(additionalArea);

            Console.WriteLine("Validation areas count after adding: " + validation.Areas.Length);

            // Ta bort det extra området
            validation.RemoveArea(additionalArea);

            Console.WriteLine("Validation areas count after removing: " + validation.Areas.Length);

            // Lägg till flera områden
            CellArea[] multipleAreas = new CellArea[]
            {
                CellArea.CreateCellArea(2, 2, 2, 2),
                CellArea.CreateCellArea(3, 3, 3, 3),
                CellArea.CreateCellArea(4, 4, 4, 4)
            };
            validation.AddAreas(multipleAreas, false, false);

            Console.WriteLine("Validation areas count after adding multiple: " + validation.Areas.Length);

            // Ta bort ett av områdena
            validation.RemoveArea(multipleAreas[1]);

            Console.WriteLine("Validation areas count after removing one: " + validation.Areas.Length);
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


