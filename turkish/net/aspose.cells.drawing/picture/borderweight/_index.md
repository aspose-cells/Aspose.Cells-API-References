---
title: "Picture.BorderWeight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture özelliği. Bir resmin kenar çizgisinin kalınlığını pt biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/picture/borderweight/
---
## Picture.BorderWeight property

Bir resmin kenar çizgisinin kalınlığını pt biriminde alır veya ayarlar.

```csharp
public double BorderWeight { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


