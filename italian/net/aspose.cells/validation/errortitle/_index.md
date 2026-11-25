---
title: "Validation.ErrorTitle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di convalida. Rappresenta il titolo della finestra di dialogo di errore della convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/errortitle/
---
## Validation.ErrorTitle property

Rappresenta il titolo della finestra di dialogo di errore di convalida dei dati.

```csharp
public string ErrorTitle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyErrorTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(0, 0, 1, 1))];
            
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 3 and 1234";
            validation.ShowError = true;

            workbook.Save("ValidationErrorTitleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


