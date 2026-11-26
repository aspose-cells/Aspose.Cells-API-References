---
title: "Axis.Title"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Получает заголовок этой оси в диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/axis/title/
---
## Axis.Title property

Получает заголовок этой оси в диаграмме.

```csharp
public Title Title { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTitleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Настроить заголовки
            chart.Title.Text = "Sample Chart";
            chart.Title.IsVisible = true;
            chart.Title.Font.Name = "Arial";
            chart.Title.Font.Size = 14;
            
            // Настроить заголовки осей
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.IsVisible = true;
            chart.CategoryAxis.Title.Font.Name = "Arial";
            
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.IsVisible = true;
            chart.ValueAxis.Title.Font.Name = "Arial";
            
            // Сохраните книгу
            workbook.Save("AxisPropertyTitleDemo_Output.xlsx");
        }
    }
}
```

### См. также

* class [Title](../../title/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


