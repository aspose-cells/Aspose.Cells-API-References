---
title: "Enum ValidationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ValidationType-Enum. Stellt den Datengültigkeitstyp dar"
type: docs
url: /de/net/aspose.cells/validationtype/
---
## ValidationType enumeration

Stellt den Typ der Datenvalidierung dar.

```csharp
public enum ValidationType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| AnyValue | `0` | Gültigkeitstyp für beliebige Werte. |
| WholeNumber | `1` | Gültigkeitstyp für ganze Zahlen. |
| Decimal | `2` | Gültigkeitstyp für Dezimalzahlen. |
| List | `3` | Gültigkeitstyp für Listen. |
| Date | `4` | Gültigkeitstyp für Datum. |
| Time | `5` | Gültigkeitstyp für Zeit. |
| TextLength | `6` | Gültigkeitstyp für Textlänge. |
| Custom | `7` | Benutzerdefinierter Gültigkeitstyp. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationTypeDemo
    {
        public static void ValidationTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Validierung zum Arbeitsblatt hinzu
            ValidationCollection validations = worksheet.Validations;
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            Validation validation = validations[validations.Add(area)];

            // Setzen Sie den Validierungstyp auf WholeNumber
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";

            // Legen Sie zusätzliche Eigenschaften für die Validierung fest
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;

            // Speichere die Arbeitsmappe
            workbook.Save("ValidationTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


