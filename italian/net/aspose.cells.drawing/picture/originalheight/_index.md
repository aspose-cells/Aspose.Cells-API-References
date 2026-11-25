---
title: "Picture.OriginalHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene l'altezza originale dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picture/originalheight/
---
## Picture.OriginalHeight property

Ottiene l'altezza originale dell'immagine.

```csharp
public int OriginalHeight { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];

            // Ottieni e visualizza l'altezza originale dell'immagine
            int originalHeight = pic.OriginalHeight;
            Console.WriteLine("Original height of the picture: " + originalHeight + " pixels");

            // Salva la cartella di lavoro
            workbook.Save("result.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


