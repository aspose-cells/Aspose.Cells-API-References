---
title: "TilePicOption.ScaleY"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TilePicOption. Получает или задает масштаб по оси Y для мозаичной картинки"
type: docs
url: /ru/net/aspose.cells.drawing/tilepicoption/scaley/
---
## TilePicOption.ScaleY property

Получает или задает масштаб по оси Y для изображения замощения.

```csharp
public double ScaleY { get; set; }
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
    public class TilePicOptionPropertyScaleYDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите текстурную заливку с изображением
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("example.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            
            // Настройте параметры мозаики с помощью ScaleY
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            
            // Сохраните книгу
            workbook.Save("TilePicOptionScaleYDemo.xlsx");
        }
    }
}
```

### См. также

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


