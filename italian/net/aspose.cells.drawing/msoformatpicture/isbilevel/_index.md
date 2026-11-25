---
title: "MsoFormatPicture.IsBiLevel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MsoFormatPicture property. Indica se quest'immagine deve essere visualizzata in bi-colore bianco e nero"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/isbilevel/
---
## MsoFormatPicture.IsBiLevel property

Indica se questa immagine deve essere visualizzata in bianco e nero a due colori.

```csharp
public bool IsBiLevel { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsBiLevelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'immagine al foglio di lavoro
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Imposta l'immagine a bi-level (bianco e nero)
            picture.FormatPicture.IsBiLevel = true;
            
            // Verifica e visualizza il valore della proprietà IsBiLevel
            Console.WriteLine("Picture is bi-level: " + picture.FormatPicture.IsBiLevel);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


