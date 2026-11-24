---
title: "FillFormat.ImageData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Gibt die Bilddaten zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/fillformat/imagedata/
---
## FillFormat.ImageData property

Liest und setzt die Bilddaten.

```csharp
public byte[] ImageData { get; set; }
```

### Hinweise

Wenn das Füllformat kein benutzerdefiniertes Texturformat ist, wird null zurückgegeben.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyImageDataDemo
    {
        public static void Run()
        {
            // Arbeitsmappe erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielbild zum Arbeitsblatt hinzufügen
            string imagePath = "example.png";
            worksheet.Pictures.Add(0, 0, imagePath);

            // Kommentar erstellen und Bilddaten festlegen
            var comment = worksheet.Comments[worksheet.Comments.Add(2, 5)];
            byte[] imageData = File.ReadAllBytes(imagePath);
            comment.CommentShape.Fill.ImageData = imageData;

            // Arbeitsmappe speichern.
            workbook.Save("FillFormatPropertyImageDataDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


