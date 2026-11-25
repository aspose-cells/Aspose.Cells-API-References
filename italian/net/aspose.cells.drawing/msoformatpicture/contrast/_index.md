---
title: "MsoFormatPicture.Contrast"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFormatPicture. Rappresenta la modifica del contrasto per l'immagine in unità percentuale"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/contrast/
---
## MsoFormatPicture.Contrast property

Rappresenta la modifica del contrasto dell'immagine in unità di percentuale.

```csharp
public double Contrast { get; set; }
```

### Osservazioni

È compreso tra -100% e 100%. Funziona allo stesso modo di Excel 2007 o versioni successive.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyContrastDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            var picture = worksheet.Pictures[pictureIndex];

            // Imposta e ottieni il valore del contrasto
            picture.FormatPicture.Contrast = 50;
            Console.WriteLine("Current contrast: " + picture.FormatPicture.Contrast);

            // Modifica il contrasto
            picture.FormatPicture.Contrast = 75;
            Console.WriteLine("Modified contrast: " + picture.FormatPicture.Contrast);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


