---
title: "Picture.OriginalHeightCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture property. Resmin orijinal yüksekliğini santimetre biriminde alır"
type: docs
url: /tr/net/aspose.cells.drawing/picture/originalheightcm/
---
## Picture.OriginalHeightCM property

Resmin orijinal yüksekliğini santimetre biriminde alır.

```csharp
public double OriginalHeightCM { get; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


