---
title: "MsoFormatPicture.RightCropInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFormatPicture. Rappresenta la posizione destra del rettangolo di ritaglio espressa in unità di pollici"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/rightcropinch/
---
## MsoFormatPicture.RightCropInch property

Rappresenta la posizione del bordo destro del rettangolo di ritaglio, in unità di pollici.

```csharp
public double RightCropInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyRightCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi un'immagine (sostituisci con il percorso reale dell'immagine)
            int pictureIndex = sheet.Pictures.Add(1, 1, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // Accedi e imposta la proprietà RightCropInch
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.RightCropInch = 0.3; // Crop 0.3 inches from right

            // Salva la cartella di lavoro
            workbook.Save("RightCropInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


