---
title: "Validation.Operator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Eigenschaft. Stellt den Operator für die Datenvalidierung dar."
type: docs
url: /de/net/aspose.cells/validation/operator/
---
## Validation.Operator property

Stellt den Operator für die Datenvalidierung dar.

```csharp
public OperatorType Operator { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyOperatorDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten für die Validierung hinzu.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Erstellen Sie einen Validierungsbereich.
            CellArea area = CellArea.CreateCellArea("B1", "B5");
            int validationIndex = worksheet.Validations.Add(area);
            Validation validation = worksheet.Validations[validationIndex];

            // Setzen Sie die Validierungseigenschaften mit einer Operator-Demonstration.
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "30";
            validation.ShowError = true;
            validation.ErrorMessage = "Value must be between 10 and 30";

            // Speichere die Arbeitsmappe
            workbook.Save("ValidationOperatorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


