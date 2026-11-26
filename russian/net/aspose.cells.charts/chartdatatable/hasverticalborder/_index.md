---
title: "ChartDataTable.HasVerticalBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartDataTable. True, если у таблицы данных диаграммы есть вертикальные границы ячеек"
type: docs
url: /ru/net/aspose.cells.charts/chartdatatable/hasverticalborder/
---
## ChartDataTable.HasVerticalBorder property

Истина, если у таблицы данных диаграммы есть вертикальные границы ячеек

```csharp
public bool HasVerticalBorder { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasVerticalBorderDemo
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

            // Показать таблицу данных
            chart.ShowDataTable = true;
            
            // Получить доступ к таблице данных через свойство ChartDataTable
            ChartDataTable dataTable = chart.ChartDataTable;

            // Продемонстрировать свойство HasVerticalBorder
            Console.WriteLine("Initial HasVerticalBorder value: " + dataTable.HasVerticalBorder);
            
            // Переключить вертикальные границы
            dataTable.HasVerticalBorder = true;
            Console.WriteLine("After setting HasVerticalBorder to true: " + dataTable.HasVerticalBorder);
            
            dataTable.HasVerticalBorder = false;
            Console.WriteLine("After setting HasVerticalBorder to false: " + dataTable.HasVerticalBorder);

            // Сохраните книгу
            workbook.Save("ChartDataTable_HasVerticalBorderDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


