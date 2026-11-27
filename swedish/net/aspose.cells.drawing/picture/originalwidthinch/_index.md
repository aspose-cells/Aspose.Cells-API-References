---
title: "Picture.OriginalWidthInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskap. Hämtar den ursprungliga bredden på bilden i tum"
type: docs
url: /sv/net/aspose.cells.drawing/picture/originalwidthinch/
---
## Picture.OriginalWidthInch property

Hämtar bildens ursprungliga bredd i tum.

```csharp
public double OriginalWidthInch { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en bild (ersätt "example.jpg" med din faktiska bildsökväg)
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            // Hämta och visa ursprunglig bredd i tum
            double picWidthInch = pic.OriginalWidthInch;
            Console.WriteLine($"Original picture width: {picWidthInch} inches");
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


