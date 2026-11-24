---
title: "Cell.GetValidationValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt den Wert der Validierung zurück, die auf diese Zelle angewendet wurde"
type: docs
url: /de/net/aspose.cells/cell/getvalidationvalue/
---
## Cell.GetValidationValue method

Liefert den Wert der Validierung, die auf diese Zelle angewendet wurde.

```csharp
public bool GetValidationValue()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationValueDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Validierungsbereich.
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.TextLength;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "5";

            // Validierung auf Zelle A1 anwenden
            Cell cell = worksheet.Cells["A1"];
            validation.AddArea(new CellArea { StartRow = cell.Row, StartColumn = cell.Column, EndRow = cell.Row, EndColumn = cell.Column });

            // Gültige Werte testen
            string[] validValues = { "a", " ab", "cd ", " xyz " };
            foreach (string value in validValues)
            {
                cell.PutValue(value);
                Console.WriteLine($"Value: '{value}' - Valid: {cell.GetValidationValue()}");
            }

            // Ungültigen Wert testen
            string invalidValue = "toolong";
            cell.PutValue(invalidValue);
            Console.WriteLine($"Value: '{invalidValue}' - Valid: {cell.GetValidationValue()}");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


