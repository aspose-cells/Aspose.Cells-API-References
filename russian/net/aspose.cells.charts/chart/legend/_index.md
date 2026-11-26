---
title: "Chart.Legend"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает легенду диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/legend/
---
## Chart.Legend property

Получает легенду диаграммы.

```csharp
public Legend Legend { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyLegendDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Настроить легенду
            chart.Legend.IsAutomaticSize = false;
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.Width = 400;
            chart.Legend.Height = 50;
            chart.Legend.Font.Size = 12;
            chart.Legend.Font.IsBold = true;

            // Сохраните книгу
            workbook.Save("ChartLegendDemo.xlsx");
        }
    }
}
```

### См. также

* class [Legend](../../legend/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


