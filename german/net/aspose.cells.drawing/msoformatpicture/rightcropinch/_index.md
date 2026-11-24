---
title: "MsoFormatPicture.RightCropInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt die Position der rechten Seite des Zuschneide-Rechtecks in Zoll an"
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/rightcropinch/
---
## MsoFormatPicture.RightCropInch property

Stellt die Position der rechten Seite des Zuschneide‑Rechtecks dar, in Zoll.

```csharp
public double RightCropInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyRightCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie ein Bild hinzu (ersetzen Sie es durch den tatsächlichen Bildpfad)
            int pictureIndex = sheet.Pictures.Add(1, 1, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // Zugriff auf und Festlegen der RightCropInch-Eigenschaft
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.RightCropInch = 0.3; // Crop 0.3 inches from right

            // Speichere die Arbeitsmappe
            workbook.Save("RightCropInchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


