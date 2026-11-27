---
title: "PageSetup.SetFooterPicture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Ställer in en bild i sidfoten på ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/pagesetup/setfooterpicture/
---
## PageSetup.SetFooterPicture method

Ställer in en bild i sidfoten på ett kalkylblad.

```csharp
public Picture SetFooterPicture(int section, byte[] footerPicture)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |
| footerPicture | Byte[] | Bilddata. |

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

    public class PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Läs in en bildfil i en byte‑array
            byte[] footerImageData = File.ReadAllBytes("footer_logo.png");
            
            try
            {
                // Anropa SetFooterPicture-metoden med sektionsindex (0 för centrerad, 1 för vänster, 2 för höger) och bilddata
                Picture footerPicture = worksheet.PageSetup.SetFooterPicture(0, footerImageData);
                
                // Ställ in sidfotstexten för att visas tillsammans med bilden
                worksheet.PageSetup.SetFooter(0, "&G");
                
                Console.WriteLine("SetFooterPicture method executed successfully with parameters (Int32, Byte[])");
                
                // Spara arbetsboken för att se sidfotsbilden
                workbook.Save("PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFooterPicture method: {ex.Message}");
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


