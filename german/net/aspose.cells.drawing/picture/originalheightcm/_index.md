---
title: "Picture.OriginalHeightCM"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Gibt die ursprüngliche Höhe des Bildes in Zentimetern zurück"
type: docs
url: /de/net/aspose.cells.drawing/picture/originalheightcm/
---
## Picture.OriginalHeightCM property

Liest die ursprüngliche Höhe des Bildes, in der Einheit Zentimeter.

```csharp
public double OriginalHeightCM { get; }
```

### Beispiele

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

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


