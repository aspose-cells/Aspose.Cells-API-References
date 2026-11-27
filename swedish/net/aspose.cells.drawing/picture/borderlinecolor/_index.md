---
title: "Picture.BorderLineColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskapen. Representerar färgen på bildens kantlinje"
type: docs
url: /sv/net/aspose.cells.drawing/picture/borderlinecolor/
---
## Picture.BorderLineColor property

Representerar färgen på bildens kantlinje.

```csharp
public Color BorderLineColor { get; set; }
```

### Exempel

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

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


