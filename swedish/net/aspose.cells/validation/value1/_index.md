---
title: "Validation.Value1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation-egenskap. Representerar det första värdet som är associerat med datavalideringen"
type: docs
url: /sv/net/aspose.cells/validation/value1/
---
## Validation.Value1 property

Representerar det första värdet som är associerat med data validation.

```csharp
public object Value1 { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyValue1Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en validering i cell A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            validation.Type = ValidationType.List;
            
            // Ange Value1-egenskapen med en strängarray
            validation.Value1 = new object[] { "Option1", "Option2", "Option3" };

            // Hämta och visa valideringsvärdena
            object[] values = validation.Value1 as object[];
            Console.WriteLine("Validation values in A1:");
            foreach (object value in values)
            {
                Console.WriteLine(value.ToString());
            }

            // Skapa en annan validering i cell B1 med olika värden
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Value1 = new object[] { "Yes", "No", "Maybe" };

            // Hämta och visa de andra valideringsvärdena
            object[] values2 = validation2.Value1 as object[];
            Console.WriteLine("\nValidation values in B1:");
            foreach (object value in values2)
            {
                Console.WriteLine(value.ToString());
            }
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


