---
title: "Picture.OriginalHeightInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture özelliği. Resmin orijinal yüksekliğini inç biriminde alır"
type: docs
url: /tr/net/aspose.cells.drawing/picture/originalheightinch/
---
## Picture.OriginalHeightInch property

Resmin orijinal yüksekliğini inç biriminde alır.

```csharp
public double OriginalHeightInch { get; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


