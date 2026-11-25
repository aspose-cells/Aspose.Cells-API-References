---
title: "MsoFormatPicture.BottomCropInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MsoFormatPicture property. Rappresenta la posizione del bordo inferiore del rettangolo di ritaglio espressa in unità di pollici"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/bottomcropinch/
---
## MsoFormatPicture.BottomCropInch property

Rappresenta la posizione del bordo inferiore del rettangolo di ritaglio, in unità di pollici.

```csharp
public double BottomCropInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBottomCropInchDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro (usando un percorso segnaposto)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Accedi all'oggetto MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Imposta la proprietà BottomCropInch e dimostra il suo utilizzo
            formatPicture.BottomCropInch = 0.3;
            formatPicture.TopCropInch = 0.2;
            
            // Salva la cartella di lavoro
            workbook.Save("MsoFormatPictureBottomCropDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


