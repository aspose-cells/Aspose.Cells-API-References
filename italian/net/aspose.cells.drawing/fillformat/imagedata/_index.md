---
title: "FillFormat.ImageData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Ottiene e imposta i dati dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/imagedata/
---
## FillFormat.ImageData property

Ottiene e imposta i dati dell'immagine.

```csharp
public byte[] ImageData { get; set; }
```

### Osservazioni

Se il formato di riempimento non è un formato texture personalizzato, restituisce null.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyImageDataDemo
    {
        public static void Run()
        {
            // Crea cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine di esempio al foglio di lavoro
            string imagePath = "example.png";
            worksheet.Pictures.Add(0, 0, imagePath);

            // Crea un commento e imposta i dati dell'immagine
            var comment = worksheet.Comments[worksheet.Comments.Add(2, 5)];
            byte[] imageData = File.ReadAllBytes(imagePath);
            comment.CommentShape.Fill.ImageData = imageData;

            // Salva cartella di lavoro
            workbook.Save("FillFormatPropertyImageDataDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


