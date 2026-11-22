---
title: "Picture.OriginalHeightInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تحصل على الارتفاع الأصلي للصورة بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells.drawing/picture/originalheightinch/
---
## Picture.OriginalHeightInch property

يحصل على الارتفاع الأصلي للصورة، بوحدة البوصة.

```csharp
public double OriginalHeightInch { get; }
```

### أمثلة

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

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


