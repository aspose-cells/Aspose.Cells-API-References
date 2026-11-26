---
title: "TextureFill.IsTiling"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextureFill. Указывает, следует ли использовать изображение в виде плитки в качестве текстуры"
type: docs
url: /ru/net/aspose.cells.drawing/texturefill/istiling/
---
## TextureFill.IsTiling property

Указывает, использовать ли изображение плиткой в качестве текстуры.

```csharp
public bool IsTiling { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyIsTilingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите данные диаграммы
            chart.NSeries.Add("A1:B3", true);
            
            // Установить заполнение текстурой для области графика
            chart.PlotArea.Area.FillFormat.Texture = TextureType.BlueTissuePaper;
            
            // Установить свойство IsTiling
            chart.PlotArea.Area.FillFormat.TextureFill.IsTiling = true;
            
            // Проверить и вывести значение IsTiling
            Console.WriteLine("IsTiling: " + chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
            
            // Сохраните книгу
            workbook.Save("TextureFillIsTilingDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


