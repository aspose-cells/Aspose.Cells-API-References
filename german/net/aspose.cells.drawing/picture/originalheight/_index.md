---
title: "Picture.OriginalHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Gibt die ursprüngliche Höhe des Bildes zurück"
type: docs
url: /de/net/aspose.cells.drawing/picture/originalheight/
---
## Picture.OriginalHeight property

Ruft die ursprüngliche Höhe des Bildes ab.

```csharp
public int OriginalHeight { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Bild zum Arbeitsblatt hinzufügen
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];

            // Erhalte und zeige die ursprüngliche Höhe des Bildes an
            int originalHeight = pic.OriginalHeight;
            Console.WriteLine("Original height of the picture: " + originalHeight + " pixels");

            // Speichere die Arbeitsmappe
            workbook.Save("result.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


