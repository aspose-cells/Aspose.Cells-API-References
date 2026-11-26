---
title: "Chart.ShowLegend"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает или задает значение, указывающее, будет ли отображаться легенда диаграммы. По умолчанию true"
type: docs
url: /ru/net/aspose.cells.charts/chart/showlegend/
---
## Chart.ShowLegend property

Получает или задает значение, указывающее, будет ли отображена легенда диаграммы. По умолчанию — истина.

```csharp
public bool ShowLegend { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowLegendDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Отображать легенду по умолчанию (true)
            Console.WriteLine("Legend initially visible: " + chart.ShowLegend);
            
            // Скрыть легенду
            chart.ShowLegend = false;
            Console.WriteLine("Legend after setting to false: " + chart.ShowLegend);
            
            // Сохраните книгу
            workbook.Save("ChartLegendExample.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


