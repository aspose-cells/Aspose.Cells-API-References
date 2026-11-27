---
title: "PageSetup.SetPicture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Ställer in en bild i sidhuvudet/sidfoten för ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/pagesetup/setpicture/
---
## PageSetup.SetPicture method

Ställer in en bild i sidhuvudet/sidfoten på ett kalkylblad.

```csharp
public Picture SetPicture(bool isFirst, bool isEven, bool isHeader, int section, byte[] imageData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isFirst | Boolean | Anger om bilden för första sidans sidhuvud/sidfoten ska ställas in. |
| isEven | Boolean | Anger om bilden för jämna sidors sidhuvud/sidfoten ska ställas in. |
| isHeader | Boolean | Anger om bilden för sidhuvud/sidfoten ska ställas in. |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |
| imageData | Byte[] | Bilddata. |

### Returvärde

Returnerar [`Picture`](../../../aspose.cells.drawing/picture/) objekt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PageSetupMethodSetPictureWithBooleanBooleanBooleanInt32ByteDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Läs in en bildfil i en byte‑array
            byte[] imageData = File.ReadAllBytes("example.jpg");

            try
            {
                // Anropa SetPicture‑metoden för att ställa in bild i sidhuvudet
                // Parametrar: isFirstPage, isEvenPage, isHeader, section, imageData
                Picture picture = pageSetup.SetPicture(false, false, true, 1, imageData);

                // Ställ in sidhuvudstext
                pageSetup.SetHeader(1, "&G");
                
                Console.WriteLine("SetPicture method executed successfully. Header image set.");

                // Spara arbetsboken
                workbook.Save("PageSetupSetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPicture method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


