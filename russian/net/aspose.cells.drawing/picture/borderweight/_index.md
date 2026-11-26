---
title: "Picture.BorderWeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Picture. Получает или задает толщину линии границы изображения в единицах pt"
type: docs
url: /ru/net/aspose.cells.drawing/picture/borderweight/
---
## Picture.BorderWeight property

Получает или задает толщину границы изображения в пунктах (pt).

```csharp
public double BorderWeight { get; set; }
```

### Примеры

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

### См. также

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


