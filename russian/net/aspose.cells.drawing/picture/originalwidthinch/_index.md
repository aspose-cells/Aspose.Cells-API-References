---
title: "Picture.OriginalWidthInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Picture. Получает исходную ширину изображения в дюймах"
type: docs
url: /ru/net/aspose.cells.drawing/picture/originalwidthinch/
---
## Picture.OriginalWidthInch property

Получает исходную ширину изображения в дюймах.

```csharp
public double OriginalWidthInch { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить изображение (замените "example.jpg" на фактический путь к вашему изображению)
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            // Получить и отобразить исходную ширину в дюймах
            double picWidthInch = pic.OriginalWidthInch;
            Console.WriteLine($"Original picture width: {picWidthInch} inches");
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### См. также

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


