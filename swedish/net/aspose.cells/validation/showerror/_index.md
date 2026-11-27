---
title: "Validation.ShowError"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsegenskap. Anger om felmeddelandet för datavalidering ska visas när användaren anger ogiltiga data"
type: docs
url: /sv/net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

Indikerar om felmeddelandet för data validation kommer att visas när användaren anger ogiltig data.

```csharp
public bool ShowError { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowErrorDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa validering för cell A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            
            // Ställ in valideringsegenskaper
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Konfigurera felvarning
            validation.ShowError = true;
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 10 and 20";

            // Skapa en annan validering för att demonstrera egenskapskopiering
            Validation targetValidation = worksheet.Validations[worksheet.Validations.Add()];
            targetValidation.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 1, EndColumn = 0 });

            // Kopiera ShowError och relaterade egenskaper från den första valideringen
            targetValidation.ShowError = validation.ShowError;
            targetValidation.ErrorTitle = validation.ErrorTitle;
            targetValidation.ErrorMessage = validation.ErrorMessage;

            // Spara arbetsboken
            workbook.Save("ValidationShowErrorDemo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


