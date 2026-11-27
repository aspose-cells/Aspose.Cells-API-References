---
title: "Klassen PictureBulletValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.PictureBulletValue‑klass. Representerar värdet för bildpunkten"
type: docs
url: /sv/net/aspose.cells.drawing.texts/picturebulletvalue/
---
## PictureBulletValue class

Representerar värdet på bildpunkten.

```csharp
public class PictureBulletValue : BulletValue
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PictureBulletValue](picturebulletvalue/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ImageData](../../aspose.cells.drawing.texts/picturebulletvalue/imagedata/) { get; set; } | Hämtar och anger bilddata för punkten. |
| override [Type](../../aspose.cells.drawing.texts/picturebulletvalue/type/) { get; } | Hämtar typen av punktlistans värde. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class TextsClassPictureBulletValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Skapa en instans av PictureBulletValue‑klassen
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Ladda exempelbilddata (ersätt med faktisk bildsökväg)
                string imagePath = "sample.png";
                if (File.Exists(imagePath))
                {
                    bulletValue.ImageData = File.ReadAllBytes(imagePath);
                    
                    // Visa grundläggande information
                    Console.WriteLine($"PictureBulletValue created with Type: {bulletValue.Type}");
                    Console.WriteLine($"Image data length: {bulletValue.ImageData?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Sample image not found, using empty bullet value");
                }
                
                // Spara arbetsboken
                workbook.Save("PictureBulletValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PictureBulletValue: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


