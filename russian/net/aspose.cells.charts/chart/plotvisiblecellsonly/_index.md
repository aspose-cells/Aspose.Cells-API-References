---
title: "Chart.PlotVisibleCellsOnly"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Указывает, отображать ли только видимые ячейки"
type: docs
url: /ru/net/aspose.cells.charts/chart/plotvisiblecellsonly/
---
## Chart.PlotVisibleCellsOnly property

Указывает, отображаются ли только видимые ячейки построения.

```csharp
public bool PlotVisibleCellsOnly { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotVisibleCellsOnlyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            
            // Скрыть строку 3
            worksheet.Cells.Rows[2].IsHidden = true;
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Установить PlotVisibleCellsOnly в false (по умолчанию true)
            chart.PlotVisibleCellsOnly = false;
            
            // Сохраните книгу
            workbook.Save("ChartPlotVisibleCellsOnlyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


