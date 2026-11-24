---
title: "PicFormatOption.Scale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PicFormatOption-Eigenschaft. Liest oder schreibt, wie das Bild gestapelt und skaliert wird"
type: docs
url: /de/net/aspose.cells.drawing/picformatoption/scale/
---
## PicFormatOption.Scale property

Liest oder legt fest, wie viele das Bild stapelt und mit welchem Maßstab.

```csharp
public double Scale { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO; // Added to resolve Stream-related issues

    public class PicFormatOptionPropertyScaleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein 1×1‑Pixel‑BMP‑Bild als Byte‑Array
            byte[] bmpBytes = new byte[]
            {
                0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
                0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
                0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00
            };

            // Füge das Bild dem Arbeitsblatt mithilfe von MemoryStream hinzu
            int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes)); // Fixed Stream conversion
            Picture picture = worksheet.Pictures[pictureIndex];

            // Konfiguriere die Bildposition und -größe
            picture.UpperLeftRow = 0;
            picture.UpperLeftColumn = 0;
            picture.LowerRightRow = 1;
            picture.LowerRightColumn = 1;

            // Hole die Texturfüllung über die FillFormat‑Eigenschaft
            TextureFill textureFill = picture.Fill.TextureFill; // Fixed cast error
            textureFill.PicFormatOption.Type = FillPictureType.Stack;

            // Zeige die Scale‑Eigenschaft an und ändere sie
            PicFormatOption picFormat = textureFill.PicFormatOption;
            Console.WriteLine("Current Scale value: " + picFormat.Scale);
            picFormat.Scale = 0.5;
            Console.WriteLine("Modified Scale value: " + picFormat.Scale);

            // Zellabmessungen erweitern, um den Effekt zu visualisieren
            worksheet.Cells.SetRowHeight(0, 100);
            worksheet.Cells.SetColumnWidth(0, 20);

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyScaleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


