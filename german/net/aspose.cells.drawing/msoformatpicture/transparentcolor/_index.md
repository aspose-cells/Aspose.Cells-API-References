---
title: "MsoFormatPicture.TransparentColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Ruft die transparente Farbe des Bildes ab und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/transparentcolor/
---
## MsoFormatPicture.TransparentColor property

Liest und setzt die transparente Farbe des Bildes.

```csharp
public CellsColor TransparentColor { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTransparentColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein Beispielbild hinzu (unter Verwendung eines einfarbigen Rechtecks als Beispiel)
            int pictureIndex = worksheet.Pictures.Add(0, 0, "sample.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Transparente Farbe festlegen
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.Blue;
            picture.FormatPicture.TransparentColor = transparentColor;

            // Transparente Farbe abrufen und anzeigen
            CellsColor currentTransparentColor = picture.FormatPicture.TransparentColor;
            Console.WriteLine("Current transparent color: " + currentTransparentColor.Color);

            // Speichere die Arbeitsmappe
            workbook.Save("TransparentColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


