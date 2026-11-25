---
title: "Picture.IsLink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Restituisce vero se l'immagine è collegata a un file"
type: docs
url: /it/net/aspose.cells.drawing/picture/islink/
---
## Picture.IsLink property

Restituisce true se l'immagine è collegata a un file.

```csharp
public bool IsLink { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine collegata
            int linkedPictureIndex = worksheet.Pictures.Add(0, 0, "https://example.com/image.jpg");
            Picture linkedPicture = worksheet.Pictures[linkedPictureIndex];

            // Aggiungi un'immagine incorporata (usando dati di esempio)
            byte[] embeddedImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample image data
            using (MemoryStream stream = new MemoryStream(embeddedImageData))
            {
                int embeddedPictureIndex = worksheet.Pictures.Add(0, 5, stream);
                Picture embeddedPicture = worksheet.Pictures[embeddedPictureIndex];

                // Dimostra la proprietà IsLink
                Console.WriteLine("Linked picture IsLink: " + linkedPicture.IsLink);
                Console.WriteLine("Embedded picture IsLink: " + embeddedPicture.IsLink);

                // Mostra un comportamento diverso basato su IsLink
                Console.WriteLine("\nLinked picture data is null: " + (linkedPicture.Data == null));
                Console.WriteLine("Embedded picture data length: " + embeddedPicture.Data.Length);
            }
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


