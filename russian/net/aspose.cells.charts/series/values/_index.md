---
title: "Series.Values"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Представляет Y‑значения этой серии диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/series/values/
---
## Series.Values property

Представляет значения Y этого ряда диаграммы.

```csharp
public string Values { get; set; }
```

### Примечания

Чтобы получить фактические значения (соответствующие каждой точке этой серии), определяемые этим свойством, пожалуйста, используйте [`PointValues`](../pointvalues/).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить серию, используя свойство Values
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.Add("=Sheet1!$C$2:$C$4", true);

            // Установить данные категории
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // Отобразить свойство Values для каждой серии
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            Console.WriteLine("Series 2 Values: " + chart.NSeries[1].Values);

            // Сохраните книгу
            workbook.Save("SeriesPropertyValuesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


