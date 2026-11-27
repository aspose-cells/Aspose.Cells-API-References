---
title: "Fill.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Fill method. /"
type: docs
url: /sv/net/aspose.cells.drawing/fill/equals/
---
## Fill.Equals method

/

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FillMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en rektangelform i arbetsbladet
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 0, 100, 150);

                // Hämta FillFormat-objektet från formen
                FillFormat fillFormat1 = rectangle.Fill;

                // Skapa en annan form för att få ett andra FillFormat-objekt
                Shape oval = worksheet.Shapes.AddOval(3, 0, 0, 0, 100, 150);
                FillFormat fillFormat2 = oval.Fill;

                // Anropa Equals-metoden för att jämföra de två FillFormat-objekten
                bool areEqual = fillFormat1.Equals(fillFormat2);

                // Visa resultatet av jämförelsen
                Console.WriteLine($"FillFormat objects are equal: {areEqual}");

                // Visa också jämförelse med null
                bool isNullEqual = fillFormat1.Equals(null);
                Console.WriteLine($"FillFormat object equals null: {isNullEqual}");

                // Spara arbetsboken
                workbook.Save("FillEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in FillFormat Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Fill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


