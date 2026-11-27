---
title: "ThreeDFormat.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat metod."
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/equals/
---
## ThreeDFormat.Equals method

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

    public class ThreeDFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att jämföra 3D-format
            Shape shape1 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 150, 100, 100, 0, 0);

            // Hämta 3D-formaten för formerna
            ThreeDFormat format1 = shape1.ThreeDFormat;
            ThreeDFormat format2 = shape2.ThreeDFormat;

            // Konfigurera identiska 3D-inställningar
            format1.BottomBevelWidth = 10;
            format1.BottomBevelHeight = 10;
            format1.BottomBevelType = BevelType.ArtDeco;

            format2.BottomBevelWidth = 10;
            format2.BottomBevelHeight = 10;
            format2.BottomBevelType = BevelType.ArtDeco;

            try
            {
                // Anropa Equals-metoden för att jämföra 3D-formaten
                bool areEqual = format1.Equals((object)format2);

                // Visa resultatet
                Console.WriteLine($"The 3D formats are equal: {areEqual}");

                // Ändra en egenskap för att göra dem olika
                format2.BottomBevelWidth = 15;
                areEqual = format1.Equals((object)format2);
                Console.WriteLine($"After modification, the 3D formats are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("ThreeDFormatEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


