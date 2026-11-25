---
title: "Picture.BorderWeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene o imposta lo spessore della linea del bordo dell'immagine in unità di pt"
type: docs
url: /it/net/aspose.cells.drawing/picture/borderweight/
---
## Picture.BorderWeight property

Ottiene o imposta lo spessore della linea di bordo di un'immagine in unità di pt.

```csharp
public double BorderWeight { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyBorderWeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];
            
            pic.BorderLineColor = Color.Red;
            pic.BorderWeight = 3;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


