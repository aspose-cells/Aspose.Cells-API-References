---
title: "Picture.BorderLineColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture özelliği. Bir resmin kenar çizgi rengini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/picture/borderlinecolor/
---
## Picture.BorderLineColor property

Bir resmin kenar çizgisinin Rengini temsil eder.

```csharp
public Color BorderLineColor { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


