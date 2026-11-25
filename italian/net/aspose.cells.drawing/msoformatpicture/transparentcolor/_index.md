---
title: "MsoFormatPicture.TransparentColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFormatPicture. Ottiene e imposta il colore trasparente dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/transparentcolor/
---
## MsoFormatPicture.TransparentColor property

Ottiene e imposta il colore trasparente dell'immagine.

```csharp
public CellsColor TransparentColor { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine di esempio (usando un rettangolo di colore solido come esempio)
            int pictureIndex = worksheet.Pictures.Add(0, 0, "sample.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Imposta il colore trasparente
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.Blue;
            picture.FormatPicture.TransparentColor = transparentColor;

            // Ottieni e visualizza il colore trasparente
            CellsColor currentTransparentColor = picture.FormatPicture.TransparentColor;
            Console.WriteLine("Current transparent color: " + currentTransparentColor.Color);

            // Salva la cartella di lavoro
            workbook.Save("TransparentColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


