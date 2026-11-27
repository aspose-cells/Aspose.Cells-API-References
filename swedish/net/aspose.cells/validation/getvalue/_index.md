---
title: "Validation.GetValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation-metod. Hämta värdet för valideringen på den specifika cellen"
type: docs
url: /sv/net/aspose.cells/validation/getvalue/
---
## Validation.GetValue method

Hämta värdet av valideringen på den specifika cellen.

```csharp
public object GetValue(int row, int column, bool isValue1)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |
| isValue1 | Boolean | Indikerar om det första värdet hämtas. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och validering
            worksheet.Cells["A1"].PutValue("Select Item:");
            worksheet.Cells["B1"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue("Item 2");
            
            // Skapa validering för cell B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:B2";
            
            // Hämta värde med GetValue-metoden med rad, kolumn och konvertera numeriska till datum-parametrar
            object value = validation.GetValue(0, 1, false);
            
            // Skriv ut resultatet
            Console.WriteLine("Validation value: " + value.ToString());
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


