---
title: "MsoFormatPicture.TopCropInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt die Position des oberen Randes des Beschnittrechtecks in Zoll an."
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/topcropinch/
---
## MsoFormatPicture.TopCropInch property

Stellt die Position der oberen Seite des Zuschneide‑Rechtecks dar, in Zoll.

```csharp
public double TopCropInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie ein Bild hinzu (ersetzen Sie es durch den tatsächlichen Bildpfad)
            int pictureIndex = sheet.Pictures.Add(0, 0, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // Greife auf die TopCropInch-Eigenschaft zu und ändere sie
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.TopCropInch = 0.3; // Crop 0.3 inches from top
            format.BottomCropInch = 0.2; // Additional crop properties for context

            // Ergebnis speichern
            workbook.Save("TopCropInchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


