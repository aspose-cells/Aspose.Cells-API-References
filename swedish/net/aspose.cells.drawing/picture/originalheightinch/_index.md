---
title: "Picture.OriginalHeightInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskapen. Hämtar originalhöjden på bilden i tum"
type: docs
url: /sv/net/aspose.cells.drawing/picture/originalheightinch/
---
## Picture.OriginalHeightInch property

Hämtar bildens ursprungliga höjd i tum.

```csharp
public double OriginalHeightInch { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            Console.WriteLine("Original picture height in inches: " + pic.OriginalHeightInch);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


