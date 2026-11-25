---
title: "Validation.ShowInput"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Validation. Indica se il messaggio di input della convalida dei dati verrà visualizzato ogni volta che l'utente seleziona una cella nell'intervallo di convalida"
type: docs
url: /it/net/aspose.cells/validation/showinput/
---
## Validation.ShowInput property

Indica se il messaggio di input della convalida dei dati verrà visualizzato ogni volta che l'utente seleziona una cella nell'intervallo di convalida dei dati.

```csharp
public bool ShowInput { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowInputDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'area di convalida
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;

            // Aggiungi convalida
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Imposta la proprietà ShowInput
            validation.ShowInput = true;
            validation.InputTitle = "Selection";
            validation.InputMessage = "Please select Yes or No";

            validation.AddArea(area);

            // Salva la cartella di lavoro
            workbook.Save("ValidationPropertyShowInputDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


