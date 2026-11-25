---
title: "Worksheet.Pictures"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene una raccolta di Picture"
type: docs
url: /it/net/aspose.cells/worksheet/pictures/
---
## Worksheet.Pictures property

Ottiene una raccolta di [`Picture`](../../../aspose.cells.drawing/picture/).

```csharp
public PictureCollection Pictures { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPicturesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Imposta le proprietà di Picture
            picture.Placement = PlacementType.FreeFloating;
            picture.BorderLineColor = System.Drawing.Color.Blue;
            picture.BorderWeight = 1;

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Carica la cartella di lavoro salvata per verificare
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Number of pictures: " + loadedWorkbook.Worksheets[0].Pictures.Count);
        }
    }
}
```

### Vedi anche

* class [PictureCollection](../../../aspose.cells.drawing/picturecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


