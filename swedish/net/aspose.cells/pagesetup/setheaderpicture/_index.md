---
title: "PageSetup.SetHeaderPicture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Ställer in en bild i rubriken på ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/pagesetup/setheaderpicture/
---
## PageSetup.SetHeaderPicture method

Ställer in en bild i sidhuvudet på ett kalkylblad.

```csharp
public Picture SetHeaderPicture(int section, byte[] headerPicture)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |
| headerPicture | Byte[] | Bilddata. |

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

    public class PageSetupMethodSetHeaderPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Läs in en bildfil i en byte‑array
            byte[] headerImageBytes = File.ReadAllBytes("header_logo.png");
            
            try
            {
                // Anropa SetHeaderPicture med sektionsindex (0 för centerrubrik) och bildbytes
                Picture picture = worksheet.PageSetup.SetHeaderPicture(0, headerImageBytes);
                
                // Ställ in rubrikskript för att visa bilden
                worksheet.PageSetup.SetHeader(0, "&G");
                
                Console.WriteLine("SetHeaderPicture method executed successfully with parameters (Int32, Byte[])");
                Console.WriteLine($"Picture dimensions: {picture.OriginalWidth}x{picture.OriginalHeight} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetHeaderPicture method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("SetHeaderPictureDemo.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


