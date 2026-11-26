---
title: "TextureFill.ImageData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextureFill. Получает и задает данные изображения заливки"
type: docs
url: /ru/net/aspose.cells.drawing/texturefill/imagedata/
---
## TextureFill.ImageData property

Получает и задает данные изображения заливки.

```csharp
public byte[] ImageData { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyImageDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить тип заливки текстурой
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;

            // Загрузить данные изображения
            byte[] imageData = File.ReadAllBytes("texture.png");

            // Установить данные изображения для заливки текстурой
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Сохраните книгу
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


