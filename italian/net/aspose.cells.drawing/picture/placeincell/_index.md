---
title: "Picture.PlaceInCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Picture. Posiziona questa immagine nella cella"
type: docs
url: /it/net/aspose.cells.drawing/picture/placeincell/
---
## Picture.PlaceInCell method

Posiziona questa immagine nella cella

```csharp
[Obsolete("Use Picture.IsPlacedInCell property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void PlaceInCell()
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Picture.IsPlacedInCell. Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodPlaceInCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Posiziona l'immagine nella cella A1
            picture.PlaceInCell();

            // Verifica che l'immagine sia posizionata nella cella
            Cell cell = worksheet.Cells["A1"];
            byte[] imageData = cell.EmbeddedImage;
            Console.WriteLine("Image placed in cell A1. Image data length: " + imageData.Length);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


