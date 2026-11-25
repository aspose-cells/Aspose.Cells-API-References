---
title: "MsoFormatPicture.TopCropInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFormatPicture. Rappresenta la posizione superiore del rettangolo di ritaglio espressa in unità di pollici"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/topcropinch/
---
## MsoFormatPicture.TopCropInch property

Rappresenta la posizione del bordo superiore del rettangolo di ritaglio, in unità di pollici.

```csharp
public double TopCropInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi un'immagine (sostituisci con il percorso reale dell'immagine)
            int pictureIndex = sheet.Pictures.Add(0, 0, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // Accedi e modifica la proprietà TopCropInch
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.TopCropInch = 0.3; // Crop 0.3 inches from top
            format.BottomCropInch = 0.2; // Additional crop properties for context

            // Salva il risultato
            workbook.Save("TopCropInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


