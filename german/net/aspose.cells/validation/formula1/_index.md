---
title: "Validation.Formula1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Eigenschaft. Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist"
type: docs
url: /de/net/aspose.cells/validation/formula1/
---
## Validation.Formula1 property

Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist.

```csharp
public string Formula1 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula1Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Listenvalidierung hinzufügen mit Formula1 als kommagetrennte Werte
            Validation validation1 = worksheet.Validations[worksheet.Validations.Add()];
            validation1.Type = ValidationType.List;
            validation1.AlertStyle = ValidationAlertType.Stop;
            validation1.Formula1 = "A,B,C";
            validation1.AddArea(new CellArea() { StartRow = 0, StartColumn = 0, EndRow = 5, EndColumn = 0 });

            // Formelvalidierung hinzufügen mit Formula1 als Zellreferenz
            Validation validation2 = worksheet.Validations[worksheet.Validations.Add()];
            validation2.Type = ValidationType.Custom;
            validation2.AlertStyle = ValidationAlertType.Stop;
            validation2.Formula1 = "=A5";
            validation2.AddArea(new CellArea() { StartRow = 0, StartColumn = 1, EndRow = 5, EndColumn = 1 });

            // Speichern und neu laden, um die Persistenz zu überprüfen
            string outputPath = "output_validation_formula1.xlsx";
            workbook.Save(outputPath);

            // Neu laden, um zu überprüfen
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            Console.WriteLine("Validation 1 Formula1: " + loadedSheet.Validations[0].Formula1);
            Console.WriteLine("Validation 2 Formula1: " + loadedSheet.Validations[1].Formula1);
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


