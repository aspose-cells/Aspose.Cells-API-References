---
title: "Validation.ErrorMessage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di convalida. Rappresenta il messaggio di errore della convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/errormessage/
---
## Validation.ErrorMessage property

Rappresenta il messaggio di errore di convalida dei dati.

```csharp
public string ErrorMessage { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyErrorMessageDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una convalida per la cella A1
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";

            // Imposta le proprietà del messaggio di errore
            validation.ErrorMessage = "Value must be between 10 and 20";
            validation.ErrorTitle = "Invalid Input";
            validation.AlertStyle = ValidationAlertType.Stop;

            // Applica la convalida e testala
            worksheet.Cells["A1"].PutValue(5); // Invalid value
            Console.WriteLine("Validation Error Message: " + validation.ErrorMessage);

            // Salva la cartella di lavoro
            workbook.Save("ValidationErrorMessageDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


