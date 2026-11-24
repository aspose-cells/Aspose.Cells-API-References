---
title: "MsoFormatPicture.BottomCropInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt die Position des unteren Randes des Beschnittrechtecks in Zoll an"
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/bottomcropinch/
---
## MsoFormatPicture.BottomCropInch property

Stellt die Position des unteren Randes des Beschnittrechtecks dar, in Zoll.

```csharp
public double BottomCropInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBottomCropInchDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie dem Arbeitsblatt ein Bild hinzu (unter Verwendung eines Platzhalterpfads)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Greift auf das MsoFormatPicture‑Objekt zu
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Setzen Sie die BottomCropInch-Eigenschaft und demonstrieren Sie deren Verwendung
            formatPicture.BottomCropInch = 0.3;
            formatPicture.TopCropInch = 0.2;
            
            // Speichere die Arbeitsmappe
            workbook.Save("MsoFormatPictureBottomCropDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


