---
title: "Picture.OriginalHeightCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Picture. Возвращает исходную высоту изображения в сантиметрах"
type: docs
url: /ru/net/aspose.cells.drawing/picture/originalheightcm/
---
## Picture.OriginalHeightCM property

Получает исходную высоту изображения в сантиметрах.

```csharp
public double OriginalHeightCM { get; }
```

### Примеры

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

### См. также

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


