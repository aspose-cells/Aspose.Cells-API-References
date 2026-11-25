---
title: "Picture.OriginalHeightCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene l'altezza originale dell'immagine nell'unità di centimetri"
type: docs
url: /it/net/aspose.cells.drawing/picture/originalheightcm/
---
## Picture.OriginalHeightCM property

Ottiene l'altezza originale dell'immagine, in centimetri.

```csharp
public double OriginalHeightCM { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            Console.WriteLine("Original height of the picture (cm): " + pic.OriginalHeightCM);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


