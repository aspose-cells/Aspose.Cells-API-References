---
title: "Series.Explosion"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Series property. Расстояние открытого куска пирога от центра круговой диаграммы выражается в процентах от диаметра пирога"
type: docs
url: /ru/net/aspose.cells.charts/series/explosion/
---
## Series.Explosion property

Расстояние открытого сектора круговой диаграммы от её центра выражается в процентах от диаметра диаграммы.

```csharp
public int Explosion { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyExplosionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Добавить круговую диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию
            int seriesIndex = chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";
            
            // Получите доступ к серии и задайте explosion
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.Explosion = 15; // Set explosion value (0-100)
            
            workbook.Save("PieChartExplosionDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


