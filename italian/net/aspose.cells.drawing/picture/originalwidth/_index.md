---
title: "Picture.OriginalWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene la larghezza originale dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picture/originalwidth/
---
## Picture.OriginalWidth property

Ottiene la larghezza originale dell'immagine.

```csharp
public int OriginalWidth { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];

            // Ottieni e visualizza la larghezza originale dell'immagine
            int originalWidth = pic.OriginalWidth;
            Console.WriteLine("Original width of the picture: " + originalWidth + " pixels");

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


