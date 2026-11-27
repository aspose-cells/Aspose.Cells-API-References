---
title: "Validation.ShowInput"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsegenskap. Anger om datavalideringens inmatningsmeddelande ska visas när användaren markerar en cell i datavalideringsområdet"
type: docs
url: /sv/net/aspose.cells/validation/showinput/
---
## Validation.ShowInput property

Indikerar om inmatningsmeddelandet för data validation kommer att visas när användaren markerar en cell i data validation-intervallet.

```csharp
public bool ShowInput { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowInputDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett valideringsområde
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;

            // Lägg till validering
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Ange egenskapen ShowInput
            validation.ShowInput = true;
            validation.InputTitle = "Selection";
            validation.InputMessage = "Please select Yes or No";

            validation.AddArea(area);

            // Spara arbetsboken
            workbook.Save("ValidationPropertyShowInputDemo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


