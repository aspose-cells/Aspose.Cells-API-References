---
title: "Series.XValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Представляет X‑значения этой серии диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/series/xvalues/
---
## Series.XValues property

Представляет значения X этого ряда диаграммы.

```csharp
public string XValues { get; set; }
```

### Примечания

Только для диаграмм Scatter и Bubble. Пожалуйста, используйте [`CategoryData`](../../seriescollection/categorydata/) для других типов диаграмм, [`CategoryValues`](../categoryvalues/) используется для получения фактических значений категорий этой серии.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            var workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i+1, 0].PutValue(i+1); // X values 1-5
                worksheet.Cells[i+1, 1].PutValue((i+1)*2); // Series 1 values
                worksheet.Cells[i+1, 2].PutValue((i+1)*3); // Series 2 values
            }

            // Добавить диаграмму рассеяния
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить серию с XValues и Values
            int seriesIndex = chart.NSeries.Add("B2:B6", false);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property
            series.Name = "Series 1";

            seriesIndex = chart.NSeries.Add("C2:C6", false);
            series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property again
            series.Name = "Series 2";

            // Сохраните книгу
            workbook.Save("SeriesXValuesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


