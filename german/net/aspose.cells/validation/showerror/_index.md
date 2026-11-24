---
title: "Validation.ShowError"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validierungseigenschaft. Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, wenn der Benutzer ungültige Daten eingibt"
type: docs
url: /de/net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, sobald der Benutzer ungültige Daten eingibt.

```csharp
public bool ShowError { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowErrorDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Validierung für Zelle A1 erstellen
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            
            // Setzt Validierungseigenschaften
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Fehlermeldung konfigurieren
            validation.ShowError = true;
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 10 and 20";

            // Erstelle eine weitere Validierung, um das Kopieren von Eigenschaften zu demonstrieren
            Validation targetValidation = worksheet.Validations[worksheet.Validations.Add()];
            targetValidation.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 1, EndColumn = 0 });

            // Kopiere ShowError und zugehörige Eigenschaften von der ersten Validierung
            targetValidation.ShowError = validation.ShowError;
            targetValidation.ErrorTitle = validation.ErrorTitle;
            targetValidation.ErrorMessage = validation.ErrorMessage;

            // Speichere die Arbeitsmappe
            workbook.Save("ValidationShowErrorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


