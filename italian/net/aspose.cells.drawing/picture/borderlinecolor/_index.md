---
title: "Picture.BorderLineColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Rappresenta il colore della linea di bordo di un'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picture/borderlinecolor/
---
## Picture.BorderLineColor property

Rappresenta il colore della linea di bordo di un'immagine.

```csharp
public Color BorderLineColor { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyBorderLineColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            pic.BorderLineColor = Color.Red;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


