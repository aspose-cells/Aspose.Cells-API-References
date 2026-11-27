---
title: "Validation.GetListValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation-metod. Hämta värdet för listan av valideringen för den angivna cellen"
type: docs
url: /sv/net/aspose.cells/validation/getlistvalue/
---
## Validation.GetListValue method

Hämta värdet för listan av valideringen för den angivna cellen.

```csharp
public object GetListValue(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |

### Returvärde

Värdet för att skapa listan för denna validering för den angivna cellen. Om listan refererar till ett område, kommer det returnerade värdet att vara ett [`ReferredArea`](../../referredarea/)‑objekt; annars kan det returnerade värdet vara null, object[] eller ett enkelt objekt.

### Anmärkningar

Endast för validering vars typ är List och som har tillämpats på den angivna cellen, annars returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetListValueWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för validering
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");

            // Skapa validering för cell B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:A4";

            // Testa GetListValue med olika parametrar
            Console.WriteLine("List values:");
            for (int i = 0; i < 4; i++)
            {
                object value = validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {value}");
            }

            // Ändra till kommaseparerade värden
            validation.Formula1 = "Red,Green,Blue";
            Console.WriteLine("\nComma-separated values:");
            for (int i = 0; i < 3; i++)
            {
                object[] values = (object[])validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {string.Join(", ", values)}");
            }

            // Ändra till ett enda värde
            validation.Formula1 = "SingleValue";
            Console.WriteLine("\nSingle value:");
            object singleValue = validation.GetListValue(0, 0);
            Console.WriteLine($"Value: {singleValue}");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


