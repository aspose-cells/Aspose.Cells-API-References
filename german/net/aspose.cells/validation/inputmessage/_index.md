---
title: "Validation.InputMessage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Eigenschaft. Stellt die Eingabenachricht der Datenvalidierung dar"
type: docs
url: /de/net/aspose.cells/validation/inputmessage/
---
## Validation.InputMessage property

Stellt die Eingabenachricht der Datenvalidierung dar.

```csharp
public string InputMessage { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputMessageDemo
    {
        public static void Run()
        {
            // Arbeitsmappe erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Validierung erstellen
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Setzen Sie die Eigenschaften der Eingabenachricht.
            validation.ShowInput = true;
            validation.InputTitle = "Selection Required";
            validation.InputMessage = "Please select either Yes or No from the dropdown";

            // Speichere die Arbeitsmappe
            workbook.Save("ValidationInputMessageDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


