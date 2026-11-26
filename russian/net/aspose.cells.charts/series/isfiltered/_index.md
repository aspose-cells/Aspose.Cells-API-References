---
title: "Series.IsFiltered"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Указывает, выбрана ли серия или отфильтрована. Значение True означает, что эта серия отфильтрована и не будет отображаться на диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/series/isfiltered/
---
## Series.IsFiltered property

Указывает, выбрана ли серия или отфильтрована. Истина означает, что эта серия отфильтрована и не будет отображаться на диаграмме.

```csharp
public bool IsFiltered { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsFilteredDemo
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
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);
            worksheet.Cells["C5"].PutValue(45);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Продемонстрировать свойство IsFiltered
            Console.WriteLine("Initial Series Count: " + chart.NSeries.Count);
            
            // Отфильтровать первую серию
            chart.NSeries[0].IsFiltered = true;
            Console.WriteLine("After filtering first series: " + chart.NSeries.Count);
            
            // Отфильтровать вторую серию
            chart.NSeries[0].IsFiltered = true;
            Console.WriteLine("After filtering second series: " + chart.NSeries.Count);
            
            // Сохраните книгу
            workbook.Save("SeriesFilteredDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


