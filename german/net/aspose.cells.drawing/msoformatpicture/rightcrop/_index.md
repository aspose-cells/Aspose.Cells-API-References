---
title: "MsoFormatPicture.RightCrop"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt die Position des rechten Randes des Beschnittrechtecks an, ausgedrückt als Verhältnis zur Bildbreite."
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/rightcrop/
---
## MsoFormatPicture.RightCrop property

Stellt die Position der rechten Seite des Zuschneide‑Rechtecks dar, ausgedrückt als Verhältnis zur Bildbreite.

```csharp
public double RightCrop { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyRightCropDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Bild zum Arbeitsblatt hinzufügen
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Rufen Sie das MsoFormatPicture des Bildes ab
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;

            // Zeigen Sie den aktuellen RightCrop-Wert an
            Console.WriteLine("Current RightCrop value: " + msoFormatPicture.RightCrop);

            // Setzen Sie einen neuen RightCrop-Wert (0,2 bedeutet, dass 20 % vom rechten Rand beschnitten werden)
            msoFormatPicture.RightCrop = 0.2;
            Console.WriteLine("New RightCrop value set to: " + msoFormatPicture.RightCrop);

            // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
            workbook.Save("RightCropDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


