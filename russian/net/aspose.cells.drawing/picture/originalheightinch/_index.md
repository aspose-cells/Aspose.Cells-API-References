---
title: "Picture.OriginalHeightInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Picture свойство. Получает оригинальную высоту картинки в дюймах"
type: docs
url: /ru/net/aspose.cells.drawing/picture/originalheightinch/
---
## Picture.OriginalHeightInch property

Получает исходную высоту изображения в дюймах.

```csharp
public double OriginalHeightInch { get; }
```

### Примеры

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

### См. также

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


