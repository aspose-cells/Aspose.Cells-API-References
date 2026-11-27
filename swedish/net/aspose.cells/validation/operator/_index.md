---
title: "Validation.Operator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation-egenskap. Representerar operatorn för datavalideringen"
type: docs
url: /sv/net/aspose.cells/validation/operator/
---
## Validation.Operator property

Representerar operatorn för data validation.

```csharp
public OperatorType Operator { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyOperatorDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för validering
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Skapa ett valideringsområde
            CellArea area = CellArea.CreateCellArea("B1", "B5");
            int validationIndex = worksheet.Validations.Add(area);
            Validation validation = worksheet.Validations[validationIndex];

            // Ange valideringsegenskaper med Operator-demonstration
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "30";
            validation.ShowError = true;
            validation.ErrorMessage = "Value must be between 10 and 30";

            // Spara arbetsboken
            workbook.Save("ValidationOperatorDemo.xlsx");
        }
    }
}
```

### Se även

* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


