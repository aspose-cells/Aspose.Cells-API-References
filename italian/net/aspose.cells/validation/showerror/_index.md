---
title: "Validation.ShowError"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Validation. Indica se il messaggio di errore della convalida dei dati verrà visualizzato ogni volta che l'utente inserisce dati non validi"
type: docs
url: /it/net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

Indica se il messaggio di errore di convalida dei dati verrà visualizzato ogni volta che l'utente inserisce dati non validi.

```csharp
public bool ShowError { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowErrorDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una convalida per la cella A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            
            // Imposta le proprietà di convalida
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Configura l'avviso di errore
            validation.ShowError = true;
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 10 and 20";

            // Crea un'altra convalida per dimostrare la copia delle proprietà
            Validation targetValidation = worksheet.Validations[worksheet.Validations.Add()];
            targetValidation.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 1, EndColumn = 0 });

            // Copia ShowError e le proprietà correlate dalla prima convalida
            targetValidation.ShowError = validation.ShowError;
            targetValidation.ErrorTitle = validation.ErrorTitle;
            targetValidation.ErrorMessage = validation.ErrorMessage;

            // Salva la cartella di lavoro
            workbook.Save("ValidationShowErrorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


