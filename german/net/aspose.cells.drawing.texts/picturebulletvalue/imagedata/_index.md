---
title: "PictureBulletValue.ImageData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PictureBulletValue-Eigenschaft. Liest und setzt die Bilddaten des Aufzählungszeichens"
type: docs
url: /de/net/aspose.cells.drawing.texts/picturebulletvalue/imagedata/
---
## PictureBulletValue.ImageData property

Liest und setzt die Bilddaten des Aufzählungszeichens.

```csharp
public byte[] ImageData { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstelle eine Instanz von PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Demonstriere das Setzen und Abrufen von ImageData
                byte[] sampleImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample data
                bulletValue.ImageData = sampleImageData;
                
                // Zeige den Wert der ImageData-Eigenschaft an
                Console.WriteLine("ImageData length: " + (bulletValue.ImageData?.Length ?? 0) + " bytes");
                
                // Zeige die Type-Eigenschaft (nur lesbar)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


