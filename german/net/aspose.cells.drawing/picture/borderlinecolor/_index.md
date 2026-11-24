---
title: "Picture.BorderLineColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Stellt die Farbe der Rahmenlinie eines Bildes dar"
type: docs
url: /de/net/aspose.cells.drawing/picture/borderlinecolor/
---
## Picture.BorderLineColor property

Stellt die Farbe der Rahmenlinie eines Bildes dar.

```csharp
public Color BorderLineColor { get; set; }
```

### Beispiele

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

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


