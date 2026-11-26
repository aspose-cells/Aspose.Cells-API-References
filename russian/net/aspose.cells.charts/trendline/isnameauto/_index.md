---
title: "Trendline.IsNameAuto"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Trendline. Возвращает, определяет ли Microsoft Excel автоматически имя линии тренда."
type: docs
url: /ru/net/aspose.cells.charts/trendline/isnameauto/
---
## Trendline.IsNameAuto property

Возвращает, определяет ли Microsoft Excel автоматически название линии тренда.

```csharp
public bool IsNameAuto { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyIsNameAutoDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавьте серию к диаграмме.
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Добавьте линию тренда — изменено для обеспечения правильного создания объекта Trendline.
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Продемонстрируйте свойство IsNameAuto.
            Console.WriteLine("Initial IsNameAuto value: " + trendline.IsNameAuto);
            
            // Установите пользовательское имя (отключает автоматическое именование).
            trendline.Name = "Custom Trendline Name";
            Console.WriteLine("After setting custom name, IsNameAuto: " + trendline.IsNameAuto);
            
            // Сбросьте к автоматическому имени.
            trendline.IsNameAuto = true;
            Console.WriteLine("After setting IsNameAuto=true, Name: " + trendline.Name);
        }
    }
}
```

### См. также

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


