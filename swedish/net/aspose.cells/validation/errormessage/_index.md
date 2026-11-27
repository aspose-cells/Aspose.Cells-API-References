---
title: "Validation.ErrorMessage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation‑egenskap. Representerar felmeddelandet för datavalidering"
type: docs
url: /sv/net/aspose.cells/validation/errormessage/
---
## Validation.ErrorMessage property

Representerar felmeddelandet för data validation.

```csharp
public string ErrorMessage { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyErrorMessageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa validering för cell A1
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

            // Ange egenskaper för felmeddelande
            validation.ErrorMessage = "Value must be between 10 and 20";
            validation.ErrorTitle = "Invalid Input";
            validation.AlertStyle = ValidationAlertType.Stop;

            // Tillämpa validering och testa den
            worksheet.Cells["A1"].PutValue(5); // Invalid value
            Console.WriteLine("Validation Error Message: " + validation.ErrorMessage);

            // Spara arbetsboken
            workbook.Save("ValidationErrorMessageDemo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


