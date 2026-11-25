---
title: "MsoFormatPicture.BottomCrop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MsoFormatPicture property. Rappresenta la posizione del bordo inferiore del rettangolo di ritaglio espressa come rapporto rispetto all'altezza dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/bottomcrop/
---
## MsoFormatPicture.BottomCrop property

Rappresenta la posizione del bordo inferiore del rettangolo di ritaglio, espressa come rapporto rispetto all'altezza dell'immagine.

```csharp
public double BottomCrop { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyBottomCropDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Ottieni il MsoFormatPicture dell'immagine
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;

            // Visualizza il valore corrente di BottomCrop
            Console.WriteLine("Current BottomCrop value: " + msoFormatPicture.BottomCrop);

            // Imposta un nuovo valore BottomCrop (0.2 significa ritagliare il 20% dal basso)
            msoFormatPicture.BottomCrop = 0.2;
            Console.WriteLine("BottomCrop set to: " + msoFormatPicture.BottomCrop);

            // Imposta altri valori di ritaglio per dimostrare l'effetto
            msoFormatPicture.TopCrop = 0.1;
            msoFormatPicture.LeftCrop = 0.1;
            msoFormatPicture.RightCrop = 0.1;

            // Salva la cartella di lavoro per vedere l'immagine ritagliata
            workbook.Save("MsoFormatPicturePropertyBottomCropDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


