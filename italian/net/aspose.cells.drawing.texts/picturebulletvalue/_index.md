---
title: "Classe PictureBulletValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Texts.PictureBulletValue. Rappresenta il valore del bullet immagine"
type: docs
url: /it/net/aspose.cells.drawing.texts/picturebulletvalue/
---
## PictureBulletValue class

Rappresenta il valore del punto elenco immagine.

```csharp
public class PictureBulletValue : BulletValue
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PictureBulletValue](picturebulletvalue/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ImageData](../../aspose.cells.drawing.texts/picturebulletvalue/imagedata/) { get; set; } | Ottiene e imposta i dati dell'immagine del bullet. |
| override [Type](../../aspose.cells.drawing.texts/picturebulletvalue/type/) { get; } | Ottiene il tipo del valore del punto elenco. |

### Esempi

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
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Crea un'istanza della classe PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Carica dati immagine di esempio (sostituisci con il percorso reale dell'immagine)
                string imagePath = "sample.png";
                if (File.Exists(imagePath))
                {
                    bulletValue.ImageData = File.ReadAllBytes(imagePath);
                    
                    // Visualizza le informazioni di base
                    Console.WriteLine($"PictureBulletValue created with Type: {bulletValue.Type}");
                    Console.WriteLine($"Image data length: {bulletValue.ImageData?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Sample image not found, using empty bullet value");
                }
                
                // Salva la cartella di lavoro
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

### Vedi anche

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


