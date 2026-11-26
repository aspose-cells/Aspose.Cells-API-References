---
title: "ChartDataTable.Border"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartDataTable. Возвращает объект Border, представляющий границу объекта"
type: docs
url: /ru/net/aspose.cells.charts/chartdatatable/border/
---
## ChartDataTable.Border property

Возвращает объект Border, который представляет границу объекта

```csharp
public Line Border { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyBorderDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Показать таблицу данных
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Настройте свойства границы
            Line border = dataTable.Border;
            border.Color = System.Drawing.Color.Blue;
            border.Style = LineType.Solid;
            border.Weight = WeightType.MediumLine;
            border.DashType = MsoLineDashStyle.Solid;
            
            // Настроить видимость границ таблицы
            dataTable.HasHorizontalBorder = true;
            dataTable.HasVerticalBorder = true;
            dataTable.HasOutlineBorder = true;

            // Сохраните книгу
            workbook.Save("ChartDataTableBorderDemo.xlsx");
        }
    }
}
```

### См. также

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


