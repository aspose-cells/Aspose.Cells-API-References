---
title: "Enum ValidationAlertType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ValidationAlertType enum. Representerar stilen för datavalideringsvarning"
type: docs
url: /sv/net/aspose.cells/validationalerttype/
---
## ValidationAlertType enumeration

Representerar varningsstilen för datavalidering.

```csharp
public enum ValidationAlertType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Information | `0` | Informationsvarningsstil. |
| Stop | `1` | Stoppvarningsstil. |
| Warning | `2` | Varningsstil. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationAlertTypeDemo
    {
        public static void ValidationAlertTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definiera ett cellområde för validering
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Lägg till en validering i kalkylbladet
            ValidationCollection validations = worksheet.Validations;
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Ställ in valideringsegenskaper
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Please enter a number between 3 and 1234.";
            validation.ShowError = true;

            // Spara arbetsboken
            workbook.Save("ValidationAlertTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


