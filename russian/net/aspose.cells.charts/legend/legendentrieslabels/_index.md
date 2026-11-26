---
title: "Legend.LegendEntriesLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Legend. Получает метки элементов легенды после вызова метода Chart.Calculate"
type: docs
url: /ru/net/aspose.cells.charts/legend/legendentrieslabels/
---
## Legend.LegendEntriesLabels property

Получает метки элементов легенды после вызова метода Chart.Calculate().

```csharp
[Obsolete("Use Legend.GetLegendLabels method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList LegendEntriesLabels { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Legend.GetLegendLabels. Это свойство будет удалено через 12 месяцев, начиная с ноября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPropertyLegendEntriesLabelsDemo
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

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы гарантировать генерацию элементов легенды
            chart.Calculate();

            // Получить легенду
            Legend legend = chart.Legend;

            // Отобразить метки элементов легенды (используя свойство)
            Console.WriteLine("Legend Entries Labels:");
            foreach (string label in legend.LegendEntriesLabels)
            {
                Console.WriteLine(label);
            }

            // Сохраните книгу
            workbook.Save("LegendEntriesLabelsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


