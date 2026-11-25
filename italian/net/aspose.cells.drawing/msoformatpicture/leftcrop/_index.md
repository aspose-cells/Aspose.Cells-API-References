---
title: "MsoFormatPicture.LeftCrop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFormatPicture. Rappresenta la posizione del lato sinistro del rettangolo di ritaglio espressa come rapporto rispetto alla larghezza dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/leftcrop/
---
## MsoFormatPicture.LeftCrop property

Rappresenta la posizione del bordo sinistro del rettangolo di ritaglio, espressa come rapporto rispetto alla larghezza dell'immagine.

```csharp
public double LeftCrop { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropDemo
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

            // Imposta la proprietà LeftCrop
            picture.FormatPicture.LeftCrop = 0.1;
            Console.WriteLine("LeftCrop set to: " + picture.FormatPicture.LeftCrop);

            // Ottieni e imposta la proprietà LeftCropInch
            double leftCropInch = picture.FormatPicture.LeftCropInch;
            picture.FormatPicture.LeftCropInch = leftCropInch;
            Console.WriteLine("LeftCropInch value: " + leftCropInch);

            // Salva la cartella di lavoro
            workbook.Save("LeftCropDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


