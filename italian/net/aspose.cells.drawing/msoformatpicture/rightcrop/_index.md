---
title: "MsoFormatPicture.RightCrop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MsoFormatPicture property. Rappresenta la posizione del bordo destro del rettangolo di ritaglio espressa come rapporto rispetto alla larghezza dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/rightcrop/
---
## MsoFormatPicture.RightCrop property

Rappresenta la posizione del bordo destro del rettangolo di ritaglio, espressa come rapporto rispetto alla larghezza dell'immagine.

```csharp
public double RightCrop { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyRightCropDemo
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

            // Visualizza il valore corrente di RightCrop
            Console.WriteLine("Current RightCrop value: " + msoFormatPicture.RightCrop);

            // Imposta un nuovo valore RightCrop (0.2 significa ritagliare il 20% da destra)
            msoFormatPicture.RightCrop = 0.2;
            Console.WriteLine("New RightCrop value set to: " + msoFormatPicture.RightCrop);

            // Salva la cartella di lavoro per vedere l'effetto
            workbook.Save("RightCropDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


