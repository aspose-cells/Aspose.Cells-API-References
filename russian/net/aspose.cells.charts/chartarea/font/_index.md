---
title: "ChartArea.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartArea. Получает объект Font указанного объекта ChartArea"
type: docs
url: /ru/net/aspose.cells.charts/chartarea/font/
---
## ChartArea.Font property

Получает объект `Font` указанного объекта ChartArea.

```csharp
public override Font Font { get; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);
            worksheet.Cells["B4"].PutValue(4000);
            worksheet.Cells["B5"].PutValue(6000);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Получить область диаграммы
            ChartArea chartArea = chart.ChartArea;
            
            // Установить свойства шрифта области диаграммы
            Aspose.Cells.Font font = chartArea.Font;
            font.Name = "Tahoma";
            font.Size = 10;
            font.Color = Color.Blue;
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;

            // Сохраните книгу
            workbook.Save("ChartAreaFontDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../../aspose.cells/font/)
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


