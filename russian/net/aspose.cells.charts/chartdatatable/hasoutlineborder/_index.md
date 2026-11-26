---
title: "ChartDataTable.HasOutlineBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartDataTable. Истина, если у таблицы данных диаграммы есть контурные границы"
type: docs
url: /ru/net/aspose.cells.charts/chartdatatable/hasoutlineborder/
---
## ChartDataTable.HasOutlineBorder property

Истина, если у таблицы данных диаграммы есть границы контура

```csharp
public bool HasOutlineBorder { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasOutlineBorderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
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

            // Показать таблицу данных и получить объект ChartDataTable
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Продемонстрировать свойство HasOutlineBorder
            dataTable.HasOutlineBorder = true; // Enable outline border
            Console.WriteLine("DataTable HasOutlineBorder: " + dataTable.HasOutlineBorder);

            // Сохраните книгу
            workbook.Save("ChartDataTableHasOutlineBorderDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


