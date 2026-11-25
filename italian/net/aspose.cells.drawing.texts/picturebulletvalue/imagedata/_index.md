---
title: "PictureBulletValue.ImageData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PictureBulletValue. Ottiene e imposta i dati immagine del bullet"
type: docs
url: /it/net/aspose.cells.drawing.texts/picturebulletvalue/imagedata/
---
## PictureBulletValue.ImageData property

Ottiene e imposta i dati dell'immagine del bullet.

```csharp
public byte[] ImageData { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea un'istanza di PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Dimostra l'impostazione e il recupero di ImageData
                byte[] sampleImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample data
                bulletValue.ImageData = sampleImageData;
                
                // Visualizza il valore della proprietà ImageData
                Console.WriteLine("ImageData length: " + (bulletValue.ImageData?.Length ?? 0) + " bytes");
                
                // Mostra la proprietà Type (sola lettura)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Salva la cartella di lavoro
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

### Vedi anche

* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


