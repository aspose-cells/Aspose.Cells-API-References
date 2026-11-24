---
title: "Klasse PictureBulletValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.PictureBulletValue Klasse. Stellt den Wert des Bildaufzählungszeichens dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/picturebulletvalue/
---
## PictureBulletValue class

Stellt den Wert der Bild‑Aufzählung dar.

```csharp
public class PictureBulletValue : BulletValue
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PictureBulletValue](picturebulletvalue/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ImageData](../../aspose.cells.drawing.texts/picturebulletvalue/imagedata/) { get; set; } | Liest und setzt die Bilddaten des Aufzählungszeichens. |
| override [Type](../../aspose.cells.drawing.texts/picturebulletvalue/type/) { get; } | Ermittelt den Typ des Aufzählungszeichenwerts. |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Erstelle eine Instanz der PictureBulletValue Klasse
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Lade Beispiel-Bilddaten (ersetze durch tatsächlichen Bildpfad)
                string imagePath = "sample.png";
                if (File.Exists(imagePath))
                {
                    bulletValue.ImageData = File.ReadAllBytes(imagePath);
                    
                    // Zeige grundlegende Informationen an
                    Console.WriteLine($"PictureBulletValue created with Type: {bulletValue.Type}");
                    Console.WriteLine($"Image data length: {bulletValue.ImageData?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Sample image not found, using empty bullet value");
                }
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


