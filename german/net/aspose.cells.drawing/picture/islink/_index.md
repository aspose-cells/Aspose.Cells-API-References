---
title: "Picture.IsLink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Gibt wahr zurück, wenn das Bild mit einer Datei verknüpft ist"
type: docs
url: /de/net/aspose.cells.drawing/picture/islink/
---
## Picture.IsLink property

Gibt true zurück, wenn das Bild mit einer Datei verknüpft ist.

```csharp
public bool IsLink { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsLinkDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein verknüpftes Bild hinzu
            int linkedPictureIndex = worksheet.Pictures.Add(0, 0, "https://example.com/image.jpg");
            Picture linkedPicture = worksheet.Pictures[linkedPictureIndex];

            // Füge ein eingebettetes Bild hinzu (unter Verwendung von Beispieldaten)
            byte[] embeddedImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample image data
            using (MemoryStream stream = new MemoryStream(embeddedImageData))
            {
                int embeddedPictureIndex = worksheet.Pictures.Add(0, 5, stream);
                Picture embeddedPicture = worksheet.Pictures[embeddedPictureIndex];

                // Demonstriere die IsLink-Eigenschaft
                Console.WriteLine("Linked picture IsLink: " + linkedPicture.IsLink);
                Console.WriteLine("Embedded picture IsLink: " + embeddedPicture.IsLink);

                // Zeige unterschiedliches Verhalten basierend auf IsLink
                Console.WriteLine("\nLinked picture data is null: " + (linkedPicture.Data == null));
                Console.WriteLine("Embedded picture data length: " + embeddedPicture.Data.Length);
            }
        }
    }
}
```

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


