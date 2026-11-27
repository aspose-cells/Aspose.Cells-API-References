---
title: "Enum ValidationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ValidationType enum. Representerar datavalideringstyp"
type: docs
url: /sv/net/aspose.cells/validationtype/
---
## ValidationType enumeration

Representerar datavalideringstyp.

```csharp
public enum ValidationType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| AnyValue | `0` | Valideringstyp för valfritt värde. |
| WholeNumber | `1` | Valideringstyp för heltal. |
| Decimal | `2` | Valideringstyp för decimal. |
| List | `3` | Valideringstyp för lista. |
| Date | `4` | Valideringstyp för datum. |
| Time | `5` | Valideringstyp för tid. |
| TextLength | `6` | Valideringstyp för textlängd. |
| Custom | `7` | Anpassad valideringstyp. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationTypeDemo
    {
        public static void ValidationTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en validering i kalkylbladet
            ValidationCollection validations = worksheet.Validations;
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            Validation validation = validations[validations.Add(area)];

            // Ställ in valideringstyp till Heltal
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";

            // Ställ in ytterligare egenskaper för valideringen
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;

            // Spara arbetsboken
            workbook.Save("ValidationTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


