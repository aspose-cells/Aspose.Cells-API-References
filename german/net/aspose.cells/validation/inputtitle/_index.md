---
title: "Validation.InputTitle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Eigenschaft. Stellt den Titel des Eingabedialogfelds für die Datenvalidierung dar."
type: docs
url: /de/net/aspose.cells/validation/inputtitle/
---
## Validation.InputTitle property

Stellt den Titel des Eingabedialogs der Datenvalidierung dar.

```csharp
public string InputTitle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputTitleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie ein Validierungsobjekt.
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.IgnoreBlank = true;
            
            // Setzen Sie den Validierungsbereich.
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Setzt Validierungseigenschaften
            validation.Formula1 = "10";
            validation.Formula2 = "100";
            validation.Operator = OperatorType.Between;
            
            // Setzen Sie die Eigenschaften der Eingabenachricht.
            validation.InputTitle = "Number Validation";
            validation.InputMessage = "Please enter a number between 10 and 100";
            
            // Speichere die Arbeitsmappe
            workbook.Save("ValidationInputTitleDemo.xlsx");
            
            // Überprüfen Sie die InputTitle-Eigenschaft.
            Console.WriteLine("Validation InputTitle: " + validation.InputTitle);
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


