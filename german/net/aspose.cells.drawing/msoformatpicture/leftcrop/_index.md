---
title: "MsoFormatPicture.LeftCrop"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt die Position der linken Seite des Beschnittrechtecks als Verhältnis zur Bildbreite an"
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/leftcrop/
---
## MsoFormatPicture.LeftCrop property

Stellt die Position der linken Seite des Zuschneide‑Rechtecks dar, ausgedrückt als Verhältnis zur Bildbreite.

```csharp
public double LeftCrop { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropDemo
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

            // LeftCrop-Eigenschaft setzen
            picture.FormatPicture.LeftCrop = 0.1;
            Console.WriteLine("LeftCrop set to: " + picture.FormatPicture.LeftCrop);

            // LeftCropInch-Eigenschaft abrufen und setzen
            double leftCropInch = picture.FormatPicture.LeftCropInch;
            picture.FormatPicture.LeftCropInch = leftCropInch;
            Console.WriteLine("LeftCropInch value: " + leftCropInch);

            // Speichere die Arbeitsmappe
            workbook.Save("LeftCropDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


