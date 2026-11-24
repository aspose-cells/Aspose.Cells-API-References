---
title: "Validation.ErrorMessage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation‑Eigenschaft. Stellt die Fehlermeldung der Datenvalidierung dar"
type: docs
url: /de/net/aspose.cells/validation/errormessage/
---
## Validation.ErrorMessage property

Stellt die Fehlermeldung der Datenvalidierung dar.

```csharp
public string ErrorMessage { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyErrorMessageDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Validierung für Zelle A1 erstellen
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";

            // Fehlermeldungs‑Eigenschaften festlegen
            validation.ErrorMessage = "Value must be between 10 and 20";
            validation.ErrorTitle = "Invalid Input";
            validation.AlertStyle = ValidationAlertType.Stop;

            // Validierung anwenden und testen
            worksheet.Cells["A1"].PutValue(5); // Invalid value
            Console.WriteLine("Validation Error Message: " + validation.ErrorMessage);

            // Speichere die Arbeitsmappe
            workbook.Save("ValidationErrorMessageDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


