---
title: "Cell.GetValidation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑metod. Hämtar valideringen som tillämpas på den här cellen"
type: docs
url: /sv/net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

Hämtar valideringen som tillämpas på den här cellen.

```csharp
public Validation GetValidation()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cell B5 och lägg till validering
            Cell cell = worksheet.Cells["B5"];
            Validation validation = cell.GetValidation();
            
            // Ange valideringstyp och visa meddelande
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            validation.ShowError = true;
            validation.ErrorMessage = "Enter value between 10 and 20";
            
            // Spara arbetsboken
            workbook.Save("ValidationDemo.xlsx");
            
            // Verifiera valideringen
            Validation retrievedValidation = cell.GetValidation();
            Console.WriteLine("Validation Type: " + retrievedValidation.Type);
            Console.WriteLine("Validation Message: " + retrievedValidation.ErrorMessage);
        }
    }
}
```

### Se även

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


