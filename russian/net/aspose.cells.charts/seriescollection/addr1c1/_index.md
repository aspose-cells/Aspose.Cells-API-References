---
title: "SeriesCollection.AddR1C1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SeriesCollection. Добавляет коллекцию Series к диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/seriescollection/addr1c1/
---
## SeriesCollection.AddR1C1 method

Добавляет коллекцию [`Series`](../../series/) к диаграмме.

```csharp
public int AddR1C1(string area, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| область | String | Указывает значения, из которых строится серия данных |
| isVertical | Boolean | Указывает, строить ли серию из диапазона ячеек по строкам или по столбцам. |

### Возвращаемое значение

Возвращает первый индекс добавленного ASeries в NSeries.

### Примечания

Если задавать данные в смежных ячейках, используйте двоеточие для их разделения. Например, R[1]C[1]:R[3]C[2]. Если задавать данные в смежных ячейках, используйте запятую для их разделения. Например, (R[1]C[1],R[3]C[2]).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddR1C1WithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet wsData = workbook.Worksheets[0];
            wsData.Name = "ChartData";

            // Пример данных
            wsData.Cells[0, 0].PutValue(1);
            wsData.Cells[1, 0].PutValue(2);
            wsData.Cells[0, 1].PutValue(3);
            wsData.Cells[1, 1].PutValue(4);

            Worksheet wsChart = workbook.Worksheets[workbook.Worksheets.Add(Aspose.Cells.SheetType.Chart)];
            wsChart.Name = "ChartSheet";

            int chartIndex = wsChart.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 0, 0, 15, 15);
            Aspose.Cells.Charts.Chart chart = wsChart.Charts[chartIndex];

            // Использование AddR1C1 с параметрами String и Boolean
            int seriesIndex = chart.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.XValues = "ChartData!R1C1:R2C1";

            workbook.Save("SeriesCollectionAddR1C1Demo.xlsx", Aspose.Cells.SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


