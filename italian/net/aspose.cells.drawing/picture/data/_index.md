---
title: "Picture.Data"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene i dati dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picture/data/
---
## Picture.Data property

Ottiene i dati dell'immagine.

```csharp
public byte[] Data { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inserisci la prima immagine
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "example1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Inserisci la seconda immagine
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "example2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Dimostra la proprietà Data copiando i dati dell'immagine
            pic2.Data = pic1.Data;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


