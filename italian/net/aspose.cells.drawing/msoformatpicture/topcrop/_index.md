---
title: "MsoFormatPicture.TopCrop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFormatPicture. Rappresenta la posizione superiore del rettangolo di ritaglio espressa come rapporto rispetto all'altezza dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/topcrop/
---
## MsoFormatPicture.TopCrop property

Rappresenta la posizione del bordo superiore del rettangolo di ritaglio, espressa come rapporto rispetto all'altezza dell'immagine.

```csharp
public double TopCrop { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropDemo
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
            
            // Imposta la proprietà TopCrop
            picture.FormatPicture.TopCrop = -6;
            
            // Restituisci il valore TopCrop
            Console.WriteLine("Picture TopCrop value: " + picture.FormatPicture.TopCrop);
            
            // Salva la cartella di lavoro
            workbook.Save("TopCropDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


