---
title: "MsoFormatPicture.Contrast"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt die Kontraständerung für das Bild in Prozent an"
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/contrast/
---
## MsoFormatPicture.Contrast property

Stellt die Kontraständerung für das Bild in Prozent dar.

```csharp
public double Contrast { get; set; }
```

### Hinweise

Sie liegt zwischen -100 % und 100 %. Sie funktioniert wie in Excel 2007 oder neueren Versionen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyContrastDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Bild zum Arbeitsblatt hinzufügen
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            var picture = worksheet.Pictures[pictureIndex];

            // Kontrastwert festlegen und abrufen
            picture.FormatPicture.Contrast = 50;
            Console.WriteLine("Current contrast: " + picture.FormatPicture.Contrast);

            // Kontrast ändern
            picture.FormatPicture.Contrast = 75;
            Console.WriteLine("Modified contrast: " + picture.FormatPicture.Contrast);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


