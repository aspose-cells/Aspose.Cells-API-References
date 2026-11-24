---
title: "MsoFormatPicture.LeftCropInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt die Position der linken Seite des Zuschneide-Rechtecks in Zoll an"
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/leftcropinch/
---
## MsoFormatPicture.LeftCropInch property

Stellt die Position der linken Seite des Zuschneide‑Rechtecks dar, in Zoll.

```csharp
public double LeftCropInch { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropInchDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];

            // Bilddaten laden
            byte[] imageData = File.ReadAllBytes("example.png");
            
            // Bild zum Arbeitsblatt hinzufügen
            int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
            var picture = sheet.Pictures[pictureIndex];

            // LeftCropInch-Eigenschaft festlegen und abrufen
            picture.FormatPicture.LeftCropInch = 0.5;
            double leftCropValue = picture.FormatPicture.LeftCropInch;

            Console.WriteLine($"Left crop value in inches: {leftCropValue}");

            // Speichere die Arbeitsmappe
            workbook.Save("LeftCropInchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


