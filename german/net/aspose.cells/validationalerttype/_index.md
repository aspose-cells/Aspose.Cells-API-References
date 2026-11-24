---
title: "Aufzählung ValidationAlertType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ValidationAlertType Aufzählung. Stellt den Stil der Datenvalidierungswarnung dar"
type: docs
url: /de/net/aspose.cells/validationalerttype/
---
## ValidationAlertType enumeration

Stellt den Alarmstil für die Datenvalidierung dar.

```csharp
public enum ValidationAlertType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Information | `0` | Informationswarnstil. |
| Stop | `1` | Stopp-Warnstil. |
| Warning | `2` | Warnungsstil. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationAlertTypeDemo
    {
        public static void ValidationAlertTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definiere einen Zellbereich für die Validierung
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Fügen Sie eine Validierung zum Arbeitsblatt hinzu
            ValidationCollection validations = worksheet.Validations;
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Setzt Validierungseigenschaften
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Please enter a number between 3 and 1234.";
            validation.ShowError = true;

            // Speichere die Arbeitsmappe
            workbook.Save("ValidationAlertTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


