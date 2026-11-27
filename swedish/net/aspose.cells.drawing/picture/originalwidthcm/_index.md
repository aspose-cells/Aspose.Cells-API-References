---
title: "Picture.OriginalWidthCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskapen. Hämtar originalbredden på bilden i centimeter"
type: docs
url: /sv/net/aspose.cells.drawing/picture/originalwidthcm/
---
## Picture.OriginalWidthCM property

Hämtar bildens ursprungliga bredd i centimeter.

```csharp
public double OriginalWidthCM { get; }
```

### Exempel

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

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


