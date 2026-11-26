---
title: "Picture.BorderLineColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Picture свойство. Представляет цвет границы линии картинки"
type: docs
url: /ru/net/aspose.cells.drawing/picture/borderlinecolor/
---
## Picture.BorderLineColor property

Представляет цвет границы изображения.

```csharp
public Color BorderLineColor { get; set; }
```

### Примеры

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

### См. также

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


