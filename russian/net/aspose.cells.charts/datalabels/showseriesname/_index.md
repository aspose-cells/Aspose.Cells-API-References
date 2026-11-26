---
title: "DataLabels.ShowSeriesName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataLabels. Указывает, отображается ли имя серии на метках данных в диаграмме. Истина — показать имя серии. Ложь — скрыть."
type: docs
url: /ru/net/aspose.cells.charts/datalabels/showseriesname/
---
## DataLabels.ShowSeriesName property

Указывает, отображается ли имя серии в метках данных на диаграмме. True — показывать имя серии. False — скрывать.

```csharp
public bool ShowSeriesName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowSeriesNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);

            // Включите метки данных для первой серии
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Включите отображение имени серии для метки данных конкретной точки
            var points = series.Points;
            points[1].DataLabels.ShowSeriesName = true;

            // Вычислить диаграмму
            chart.Calculate();

            // Сохраните книгу
            workbook.Save("DataLabelsShowSeriesNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


