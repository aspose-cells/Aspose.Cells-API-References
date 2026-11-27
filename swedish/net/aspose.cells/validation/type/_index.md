---
title: "Validation.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Valideringsegenskap. Representerar datavalideringstypen"
type: docs
url: /sv/net/aspose.cells/validation/type/
---
## Validation.Type property

Representerar typen av data validation.

```csharp
public ValidationType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en validering i cell A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.ErrorTitle = "Number Validation";
            validation.ErrorMessage = "Please enter a whole number";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });

            // Demonstrera egenskapen Type
            Console.WriteLine("Validation Type: " + validation.Type);
            
            // Spara arbetsboken
            workbook.Save("ValidationExample.xlsx");
        }
    }
}
```

### Se även

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


