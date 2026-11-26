---
title: "Chart.SecondValueAxis"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает вторую ось Y диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/secondvalueaxis/
---
## Chart.SecondValueAxis property

Получает вторую ось Y диаграммы.

```csharp
public Axis SecondValueAxis { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySecondValueAxisDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(5000);
            worksheet.Cells["C3"].PutValue(3000);
            worksheet.Cells["C4"].PutValue(1000);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Включите вторичную ось значений для второй серии
            chart.NSeries[1].PlotOnSecondAxis = true;

            // Настройте вторичную ось значений
            Axis secondValueAxis = chart.SecondValueAxis;
            secondValueAxis.Title.Text = "Secondary Axis";
            secondValueAxis.MinValue = 0;
            secondValueAxis.MaxValue = 6000;
            secondValueAxis.MajorUnit = 1000;

            // Сохраните книгу
            workbook.Save("SecondValueAxisDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


