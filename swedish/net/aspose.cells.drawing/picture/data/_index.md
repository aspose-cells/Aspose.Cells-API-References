---
title: "Picture.Data"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskap. Hämtar data för bilden"
type: docs
url: /sv/net/aspose.cells.drawing/picture/data/
---
## Picture.Data property

Hämtar bildens data.

```csharp
public byte[] Data { get; set; }
```

### Exempel

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
            
            // Infoga första bilden
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "example1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Infoga andra bilden
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "example2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Demonstrera Data-egenskapen genom att kopiera bilddata
            pic2.Data = pic1.Data;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


