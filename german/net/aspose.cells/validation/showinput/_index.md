---
title: "Validation.ShowInput"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Eigenschaft. Gibt an, ob die Eingabenachricht der Datenvalidierung angezeigt wird, wann immer der Benutzer eine Zelle im Datenvalidierungsbereich auswählt"
type: docs
url: /de/net/aspose.cells/validation/showinput/
---
## Validation.ShowInput property

Gibt an, ob die Eingabenachricht der Datenvalidierung angezeigt wird, sobald der Benutzer eine Zelle im Datenvalidierungsbereich auswählt.

```csharp
public bool ShowInput { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowInputDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Validierungsbereich
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;

            // Validierung hinzufügen
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Setze ShowInput-Eigenschaft
            validation.ShowInput = true;
            validation.InputTitle = "Selection";
            validation.InputMessage = "Please select Yes or No";

            validation.AddArea(area);

            // Speichere die Arbeitsmappe
            workbook.Save("ValidationPropertyShowInputDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


