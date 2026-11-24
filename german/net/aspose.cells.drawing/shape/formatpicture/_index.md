---
title: "Shape.FormatPicture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Ermittelt und legt die Optionen des Bildformats fest."
type: docs
url: /de/net/aspose.cells.drawing/shape/formatpicture/
---
## Shape.FormatPicture property

Liest und legt die Optionen des Bildformats fest.

```csharp
public MsoFormatPicture FormatPicture { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFormatPictureDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Bild zum Arbeitsblatt hinzufügen
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Auf die FormatPicture-Eigenschaft des Shapes zugreifen
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;
            
            // Bildformateigenschaften ändern
            msoFormatPicture.Brightness = 0.5f;
            msoFormatPicture.Contrast = 0.7f;
            msoFormatPicture.Transparency = 0.3f;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShapePropertyFormatPictureDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../../msoformatpicture/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


