---
title: "Picture.OriginalWidthCM"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Liefert die ursprüngliche Breite des Bildes in Zentimetern"
type: docs
url: /de/net/aspose.cells.drawing/picture/originalwidthcm/
---
## Picture.OriginalWidthCM property

Liest die ursprüngliche Breite des Bildes, in der Einheit Zentimeter.

```csharp
public double OriginalWidthCM { get; }
```

### Beispiele

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

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


