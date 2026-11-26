---
title: "FillFormat.Texture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "FillFormat свойство. Представляет тип текстуры для указанного заполнения"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/texture/
---
## FillFormat.Texture property

Представляет тип текстуры для указанного заполнения.

```csharp
public TextureType Texture { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTextureDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установите текстуру для третьей точки первой серии
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Oak;

            // Сохраните книгу
            workbook.Save("FillFormatTextureDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextureType](../../texturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


