---
title: "Validation.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Eigenschaft. Stellt den Typ der Datenvalidierung dar"
type: docs
url: /de/net/aspose.cells/validation/type/
---
## Validation.Type property

Stellt den Typ der Datenvalidierung dar.

```csharp
public ValidationType Type { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Validierung zu Zelle A1 hinzufügen
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.ErrorTitle = "Number Validation";
            validation.ErrorMessage = "Please enter a whole number";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });

            // Demonstriere die Type-Eigenschaft
            Console.WriteLine("Validation Type: " + validation.Type);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ValidationExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


