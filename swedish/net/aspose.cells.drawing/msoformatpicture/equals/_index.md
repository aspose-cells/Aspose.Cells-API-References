---
title: "MsoFormatPicture.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture-metod."
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/equals/
---
## MsoFormatPicture.Equals method

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

    public class MsoFormatPictureMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till två bilder i kalkylbladet
            int pictureIndex1 = worksheet.Pictures.Add(0, 0, "example.jpg");
            int pictureIndex2 = worksheet.Pictures.Add(5, 0, "example.jpg");
            
            Picture picture1 = worksheet.Pictures[pictureIndex1];
            Picture picture2 = worksheet.Pictures[pictureIndex2];

            // Hämta MsoFormatPicture-objekten
            MsoFormatPicture format1 = picture1.FormatPicture;
            MsoFormatPicture format2 = picture2.FormatPicture;

            // Ställ in olika egenskaper för att demonstrera likhetsjämförelse
            format1.Brightness = 0.5;
            format1.Contrast = 0.3;
            format2.Brightness = 0.5;
            format2.Contrast = 0.3;

            try
            {
                // Jämför de två MsoFormatPicture-objekten
                bool areEqual = format1.Equals((object)format2);
                Console.WriteLine($"Format objects are equal: {areEqual}");

                // Modifiera ett format och jämför igen
                format2.Brightness = 0.7;
                areEqual = format1.Equals((object)format2);
                Console.WriteLine($"After modification, format objects are equal: {areEqual}");

                // Jämför med null
                bool isNullEqual = format1.Equals((object)null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Jämför med annan typ
                bool isDifferentTypeEqual = format1.Equals((object)"string");
                Console.WriteLine($"Comparison with different type: {isDifferentTypeEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("MsoFormatPictureMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


