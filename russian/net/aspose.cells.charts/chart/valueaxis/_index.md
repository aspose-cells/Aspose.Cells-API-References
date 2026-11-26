---
title: "Chart.ValueAxis"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает ось Y диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/valueaxis/
---
## Chart.ValueAxis property

Получает ось Y диаграммы.

```csharp
public Axis ValueAxis { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyValueAxisDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100000000);
            worksheet.Cells["B3"].PutValue(200000000);
            worksheet.Cells["B4"].PutValue(300000000);

            // Добавьте диаграмму и задайте её диапазон данных
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Настройте свойства ValueAxis
            chart.ValueAxis.DisplayUnit = DisplayUnitType.HundredMillions;
            chart.ValueAxis.Title.Text = "Values (in 100 millions)";
            chart.ValueAxis.MajorUnit = 1;

            // Сохраните книгу
            workbook.Save("ChartPropertyValueAxisDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


