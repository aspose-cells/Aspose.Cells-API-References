---
title: "Picture.OriginalHeightInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene l'altezza originale dell'immagine in unità di pollici"
type: docs
url: /it/net/aspose.cells.drawing/picture/originalheightinch/
---
## Picture.OriginalHeightInch property

Ottiene l'altezza originale dell'immagine, in pollici.

```csharp
public double OriginalHeightInch { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            Console.WriteLine("Original picture height in inches: " + pic.OriginalHeightInch);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


