---
title: "ChartDataTable.AutoScaleFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartDataTable. True, если текст в объекте меняет размер шрифта при изменении размера объекта. Значение по умолчанию — True"
type: docs
url: /ru/net/aspose.cells.charts/chartdatatable/autoscalefont/
---
## ChartDataTable.AutoScaleFont property

True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyAutoScaleFontDemo
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

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Включить таблицу данных
            chart.ShowDataTable = true;
            
            // Получить доступ к свойствам таблицы данных диаграммы
            // Правильный способ получения ChartDataTable, когда ShowDataTable равно True
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Продемонстрировать свойство AutoScaleFont
            dataTable.AutoScaleFont = false; // Disable auto-scaling
            Console.WriteLine("AutoScaleFont (false): " + dataTable.AutoScaleFont);
            
            dataTable.AutoScaleFont = true; // Enable auto-scaling
            Console.WriteLine("AutoScaleFont (true): " + dataTable.AutoScaleFont);

            // Сохраните книгу
            workbook.Save("ChartDataTableAutoScaleFontDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


