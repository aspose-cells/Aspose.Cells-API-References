---
title: "Validation.InputTitle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Validation. Rappresenta il titolo della finestra di dialogo di input della convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/inputtitle/
---
## Validation.InputTitle property

Rappresenta il titolo della finestra di dialogo di input della convalida dei dati.

```csharp
public string InputTitle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputTitleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un oggetto di convalida
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.IgnoreBlank = true;
            
            // Imposta l'intervallo di convalida
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Imposta le proprietà di convalida
            validation.Formula1 = "10";
            validation.Formula2 = "100";
            validation.Operator = OperatorType.Between;
            
            // Imposta le proprietà del messaggio di input
            validation.InputTitle = "Number Validation";
            validation.InputMessage = "Please enter a number between 10 and 100";
            
            // Salva la cartella di lavoro
            workbook.Save("ValidationInputTitleDemo.xlsx");
            
            // Verifica la proprietà InputTitle
            Console.WriteLine("Validation InputTitle: " + validation.InputTitle);
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


