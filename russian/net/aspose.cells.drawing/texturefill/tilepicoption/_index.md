---
title: "TextureFill.TilePicOption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextureFill. Получает или задает параметр плитки изображения"
type: docs
url: /ru/net/aspose.cells.drawing/texturefill/tilepicoption/
---
## TextureFill.TilePicOption property

Получает или задает параметр мозаичной картинки.

```csharp
public TilePicOption TilePicOption { get; set; }
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
    public class TextureFillPropertyTilePicOptionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Установите текстурную заливку с изображением
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("texture.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Настроить параметры плитки
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetX = 10;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetY = 10;

            // Сохраните книгу
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [TilePicOption](../../tilepicoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


