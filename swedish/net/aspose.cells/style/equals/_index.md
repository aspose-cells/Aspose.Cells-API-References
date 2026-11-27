---
title: "Style.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style method. Bestämmer om två Style‑instanser är lika"
type: docs
url: /sv/net/aspose.cells/style/equals/
---
## Style.Equals method

Bestämmer om två Style-instanser är lika.

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object | Style‑objektet att jämföra med det aktuella Style‑objektet. |

### Returvärde

true om det angivna objektet är lika med det aktuella objektet; annars false.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två stilar för jämförelse
            Style style1 = workbook.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.HorizontalAlignment = TextAlignmentType.Center;

            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Arial";
            style2.Font.Size = 12;
            style2.HorizontalAlignment = TextAlignmentType.Center;

            try
            {
                // Anropa Equals-metoden för att jämföra stilarna
                bool areEqual = style1.Equals((object)style2);

                // Visa resultatet
                Console.WriteLine($"The styles are equal: {areEqual}");

                // Applicera stilarna för att demonstrera att de är identiska
                if (areEqual)
                {
                    Cell cell1 = worksheet.Cells["A1"];
                    cell1.PutValue("Style 1");
                    cell1.SetStyle(style1);

                    Cell cell2 = worksheet.Cells["A2"];
                    cell2.PutValue("Style 2");
                    cell2.SetStyle(style2);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("StyleEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


