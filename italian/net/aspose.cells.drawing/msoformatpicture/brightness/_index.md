---
title: "MsoFormatPicture.Brightness"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFormatPicture. Rappresenta la modifica della luminosità dell'immagine in unità percentuale"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/brightness/
---
## MsoFormatPicture.Brightness property

Rappresenta la modifica della luminosità dell'immagine in unità di percentuale.

```csharp
public double Brightness { get; set; }
```

### Osservazioni

È compreso tra -100% e 100%. Funziona allo stesso modo di Excel 2007 o versioni successive.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBrightnessDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[pictureIndex];

            // Imposta e ottieni la luminosità
            picture.FormatPicture.Brightness = 30;
            Console.WriteLine("Picture brightness: " + picture.FormatPicture.Brightness);

            // Modifica luminosità
            picture.FormatPicture.Brightness = 70;
            Console.WriteLine("Updated brightness: " + picture.FormatPicture.Brightness);
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


