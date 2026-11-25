---
title: "Validation.InputMessage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di convalida. Rappresenta il messaggio di input della convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/inputmessage/
---
## Validation.InputMessage property

Rappresenta il messaggio di input della convalida dei dati.

```csharp
public string InputMessage { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputMessageDemo
    {
        public static void Run()
        {
            // Crea cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea convalida
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Imposta le proprietà del messaggio di input
            validation.ShowInput = true;
            validation.InputTitle = "Selection Required";
            validation.InputMessage = "Please select either Yes or No from the dropdown";

            // Salva la cartella di lavoro
            workbook.Save("ValidationInputMessageDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


