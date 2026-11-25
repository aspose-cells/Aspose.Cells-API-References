---
title: "Picture.OriginalWidthCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene la larghezza originale dell'immagine in unità di centimetri"
type: docs
url: /it/net/aspose.cells.drawing/picture/originalwidthcm/
---
## Picture.OriginalWidthCM property

Ottiene la larghezza originale dell'immagine, in centimetri.

```csharp
public double OriginalWidthCM { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            Console.WriteLine("Original width of the picture in centimeters: " + pic.OriginalWidthCM);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


