---
title: "MsoFormatPicture.BottomCrop"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt die Position des unteren Randes des Beschnittrechtecks an, ausgedrückt als Verhältnis zur Bildhöhe."
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/bottomcrop/
---
## MsoFormatPicture.BottomCrop property

Stellt die Position des unteren Randes des Beschnittrechtecks dar, ausgedrückt als Verhältnis zur Bildhöhe.

```csharp
public double BottomCrop { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyBottomCropDemo
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

            // Zeigen Sie den aktuellen BottomCrop-Wert an
            Console.WriteLine("Current BottomCrop value: " + msoFormatPicture.BottomCrop);

            // Setzen Sie einen neuen BottomCrop-Wert (0,2 bedeutet, dass 20 % vom unteren Rand beschnitten werden)
            msoFormatPicture.BottomCrop = 0.2;
            Console.WriteLine("BottomCrop set to: " + msoFormatPicture.BottomCrop);

            // Setzen Sie weitere Beschnittwerte, um die Wirkung zu demonstrieren
            msoFormatPicture.TopCrop = 0.1;
            msoFormatPicture.LeftCrop = 0.1;
            msoFormatPicture.RightCrop = 0.1;

            // Speichern Sie die Arbeitsmappe, um das beschnittene Bild zu sehen
            workbook.Save("MsoFormatPicturePropertyBottomCropDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


