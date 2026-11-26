---
title: "Series.CountOfDataValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Возвращает количество значений данных"
type: docs
url: /ru/net/aspose.cells.charts/series/countofdatavalues/
---
## Series.CountOfDataValues property

Получает количество значений данных.

```csharp
public int CountOfDataValues { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyCountOfDataValuesDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            for (int i = 0; i < 4; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1); // A1:A4 with values 1-4
            }

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию, используя диапазон данных
            chart.NSeries.Add("A1:A4", true);
            
            // Отобразить количество значений данных в первой серии
            Console.WriteLine("Count of data values in series: " + chart.NSeries[0].CountOfDataValues);
            
            // Сохраните книгу
            workbook.Save("SeriesPropertyCountOfDataValuesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


