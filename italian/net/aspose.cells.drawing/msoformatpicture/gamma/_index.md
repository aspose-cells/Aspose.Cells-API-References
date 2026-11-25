---
title: "MsoFormatPicture.Gamma"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFormatPicture. Rappresenta la gamma dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/gamma/
---
## MsoFormatPicture.Gamma property

Rappresenta la gamma dell'immagine.

```csharp
public double Gamma { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyGammaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro (usando un percorso immagine di esempio)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Accedi all'oggetto MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Imposta la proprietà Gamma
            formatPicture.Gamma = 1.5; // Demonstrating Gamma adjustment

            // Salva la cartella di lavoro
            workbook.Save("MsoFormatPictureGammaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


