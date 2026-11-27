---
title: "PictureBulletValue.ImageData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PictureBulletValue egenskap. Hämtar och anger bilddata för punkten"
type: docs
url: /sv/net/aspose.cells.drawing.texts/picturebulletvalue/imagedata/
---
## PictureBulletValue.ImageData property

Hämtar och anger bilddata för punkten.

```csharp
public byte[] ImageData { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class PictureBulletValuePropertyImageDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en instans av PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Demonstrera att sätta och hämta ImageData
                byte[] sampleImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample data
                bulletValue.ImageData = sampleImageData;
                
                // Visa värdet för ImageData‑egenskapen
                Console.WriteLine("ImageData length: " + (bulletValue.ImageData?.Length ?? 0) + " bytes");
                
                // Visa Type‑egenskapen (endast läs)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Spara arbetsboken
                workbook.Save("PictureBulletValueImageDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


