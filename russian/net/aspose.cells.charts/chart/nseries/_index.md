---
title: "Chart.NSeries"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает коллекцию SeriesCollection, представляющую серии данных в диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

Возвращает коллекцию [`SeriesCollection`](../../seriescollection/), представляющую серии данных в диаграмме.

```csharp
public SeriesCollection NSeries { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNSeriesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 2, 25, 11);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            // Установите источник данных для серий диаграммы, используя NSeries
            chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);

            // Установить заголовок диаграммы
            chart.Title.Text = "NSeries Demo Chart";

            // Сохраните книгу
            workbook.Save("NSeriesDemo.xlsx");
        }
    }
}
```

### См. также

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


