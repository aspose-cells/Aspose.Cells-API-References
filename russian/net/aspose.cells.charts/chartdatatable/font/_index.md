---
title: "ChartDataTable.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartDataTable. Возвращает объект Font, который представляет настройки шрифта указанной таблицы данных диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartdatatable/font/
---
## ChartDataTable.Font property

Возвращает объект `Font`, который представляет настройки шрифта указанной таблицы данных диаграммы.

```csharp
public Font Font { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Включить таблицу данных
            chart.ShowDataTable = true;
            
            // Получить объект таблицы данных
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Настроить шрифт таблицы данных
            dataTable.Font.Size = 14;
            dataTable.Font.Color = Color.Red;
            dataTable.Font.IsBold = true;
            dataTable.Font.Name = "Arial";

            // Сохраните книгу
            workbook.Save("ChartDataTableFontDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../../aspose.cells/font/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


