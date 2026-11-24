---
title: "MsoFormatPicture.Gamma"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt das Gamma des Bildes an"
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/gamma/
---
## MsoFormatPicture.Gamma property

Stellt das Gamma des Bildes dar.

```csharp
public double Gamma { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyGammaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie ein Bild zum Arbeitsblatt hinzu (unter Verwendung eines Beispiel-Bildpfads)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Greift auf das MsoFormatPicture‑Objekt zu
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Setze die Gamma-Eigenschaft
            formatPicture.Gamma = 1.5; // Demonstrating Gamma adjustment

            // Speichere die Arbeitsmappe
            workbook.Save("MsoFormatPictureGammaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


