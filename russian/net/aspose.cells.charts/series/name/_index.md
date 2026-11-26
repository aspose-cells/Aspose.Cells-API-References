---
title: "Series.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает или задаёт имя серии данных"
type: docs
url: /ru/net/aspose.cells.charts/series/name/
---
## Series.Name property

Получает или задает имя серии данных.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Series Name");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию к диаграмме
            chart.NSeries.Add("A2:C2", true);
            
            // Продемонстрировать использование свойства Name
            // 1. Ссылка на имя ячейки
            chart.NSeries[0].Name = "=A1";
            
            // 2. Установите строку в качестве имени
            chart.NSeries[0].Name = "First Series";
            
            // Сохраните книгу
            workbook.Save("SeriesPropertyNameDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


