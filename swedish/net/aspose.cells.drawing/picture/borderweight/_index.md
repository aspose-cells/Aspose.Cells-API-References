---
title: "Picture.BorderWeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskap. Hämtar eller anger vikten på bildens kantlinje i enheter av pt"
type: docs
url: /sv/net/aspose.cells.drawing/picture/borderweight/
---
## Picture.BorderWeight property

Hämtar eller anger tjockleken på bildens kantlinje i pt.

```csharp
public double BorderWeight { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyBorderWeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];
            
            pic.BorderLineColor = Color.Red;
            pic.BorderWeight = 3;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


