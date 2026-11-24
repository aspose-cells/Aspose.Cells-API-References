---
title: "MsoFormatPicture.TopCrop"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt die Position des oberen Randes des Beschnittrechtecks als Verhältnis zur Bildhöhe an."
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/topcrop/
---
## MsoFormatPicture.TopCrop property

Stellt die Position der oberen Seite des Zuschneide‑Rechtecks dar, ausgedrückt als Verhältnis zur Bildhöhe.

```csharp
public double TopCrop { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ein Bild zum Arbeitsblatt hinzufügen
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Setze die TopCrop-Eigenschaft
            picture.FormatPicture.TopCrop = -6;
            
            // Gib den TopCrop-Wert aus
            Console.WriteLine("Picture TopCrop value: " + picture.FormatPicture.TopCrop);
            
            // Speichere die Arbeitsmappe
            workbook.Save("TopCropDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


