---
title: "MsoFormatPicture.LeftCropInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFormatPicture. Rappresenta la posizione sinistra del rettangolo di ritaglio espressa in unità di pollici"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/leftcropinch/
---
## MsoFormatPicture.LeftCropInch property

Rappresenta la posizione del bordo sinistro del rettangolo di ritaglio, in unità di pollici.

```csharp
public double LeftCropInch { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropInchDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];

            // Carica i dati dell'immagine
            byte[] imageData = File.ReadAllBytes("example.png");
            
            // Aggiungi immagine al foglio di lavoro
            int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
            var picture = sheet.Pictures[pictureIndex];

            // Imposta e ottieni la proprietà LeftCropInch
            picture.FormatPicture.LeftCropInch = 0.5;
            double leftCropValue = picture.FormatPicture.LeftCropInch;

            Console.WriteLine($"Left crop value in inches: {leftCropValue}");

            // Salva la cartella di lavoro
            workbook.Save("LeftCropInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


