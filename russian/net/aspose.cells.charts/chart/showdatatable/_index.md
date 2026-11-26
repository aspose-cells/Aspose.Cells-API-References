---
title: "Chart.ShowDataTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает или задает значение, указывающее, отображает ли диаграмма таблицу данных"
type: docs
url: /ru/net/aspose.cells.charts/chart/showdatatable/
---
## Chart.ShowDataTable property

Получает или задает значение, указывающее, отображает ли диаграмма таблицу данных.

```csharp
public bool ShowDataTable { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowDataTableDemo
    {
        public static void Run()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            dataSheet.Cells["B1"].PutValue("Column 1");
            dataSheet.Cells["C1"].PutValue("Column 2");
            dataSheet.Cells["A2"].PutValue("Item 1");
            dataSheet.Cells["A3"].PutValue("Item 2");
            dataSheet.Cells["A4"].PutValue("Item 3");
            
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["B4"].PutValue(30);
            dataSheet.Cells["C2"].PutValue(15);
            dataSheet.Cells["C3"].PutValue(25);
            dataSheet.Cells["C4"].PutValue(35);

            // Добавить лист диаграммы
            int chartIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartIndex];
            
            // Создать диаграмму
            chartSheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = chartSheet.Charts[0];
            
            // Установить источник данных
            chart.NSeries.Add("Sheet1!B2:C4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";
            
            // Включить отображение таблицы данных
            chart.ShowDataTable = true;
            
            // Сохраните книгу
            workbook.Save("ChartWithDataTable.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


