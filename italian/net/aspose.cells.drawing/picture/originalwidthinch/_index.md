---
title: "Picture.OriginalWidthInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene la larghezza originale dell'immagine in unità di pollici"
type: docs
url: /it/net/aspose.cells.drawing/picture/originalwidthinch/
---
## Picture.OriginalWidthInch property

Ottiene la larghezza originale dell'immagine, in pollici.

```csharp
public double OriginalWidthInch { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'immagine (sostituisci "example.jpg" con il percorso reale della tua immagine)
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            // Ottieni e visualizza la larghezza originale in pollici
            double picWidthInch = pic.OriginalWidthInch;
            Console.WriteLine($"Original picture width: {picWidthInch} inches");
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


