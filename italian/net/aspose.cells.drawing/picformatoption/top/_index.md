---
title: "PicFormatOption.Top"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PicFormatOption. Ottiene o imposta l'offset superiore per lo stretching dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picformatoption/top/
---
## PicFormatOption.Top property

Ottiene o imposta lo spostamento superiore per lo stretching dell'immagine.

```csharp
public double Top { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTopDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Usa un'immagine esistente o fornisci il percorso corretto dell'immagine
            string imagePath = "existingImage.png";

            // Aggiungi una forma con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
            
            // Applica il riempimento immagine usando ImageData
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);

            // Crea e configura direttamente PicFormatOption
            PicFormatOption picFormat = new PicFormatOption();

            Console.WriteLine("Initial Top value: " + picFormat.Top);
            picFormat.Top = 0.3;

            // Supponendo che PicFormatOption debba essere associato al formato di riempimento
            // Questa parte potrebbe richiedere un'implementazione specifica dell'API non mostrata nelle definizioni dei tipi
            // shape.FillFormat.SetPicFormatOption(picFormat);

            Console.WriteLine("Modified Top value: " + picFormat.Top);
            workbook.Save("TopPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


