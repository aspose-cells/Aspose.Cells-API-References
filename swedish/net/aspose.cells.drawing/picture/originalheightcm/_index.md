---
title: "Picture.OriginalHeightCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskap. Hämtar originalhöjden på bilden i enheten centimeter"
type: docs
url: /sv/net/aspose.cells.drawing/picture/originalheightcm/
---
## Picture.OriginalHeightCM property

Hämtar bildens ursprungliga höjd i centimeter.

```csharp
public double OriginalHeightCM { get; }
```

### Exempel

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

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


