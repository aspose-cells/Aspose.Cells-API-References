---
title: "Chart.PivotSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Источник — данные сводной таблицы. Если PivotSource не пуст, диаграмма является PivotChart."
type: docs
url: /ru/net/aspose.cells.charts/chart/pivotsource/
---
## Chart.PivotSource property

Источник — данные сводной таблицы. Если PivotSource не пуст, диаграмма является PivotChart.

```csharp
public string PivotSource { get; set; }
```

### Примечания

Если сводная таблица "PivotTable1" находится на листе "Sheet1" в файле "Book1.xls". pivotSource может быть "[Book1.xls]Sheet1!PivotTable1", если диаграмма и сводная таблица находятся в разных книгах. При установке этого свойства предыдущее указание источника данных будет потеряно.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPivotSourceDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;
            
            // Добавьте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить источник сводных данных для диаграммы
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Обновить данные сводной таблицы и диаграмму
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            chart.RefreshPivotData();
            
            // Сохраните книгу
            workbook.Save("PivotSourceDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Chart PivotSource demo executed successfully.");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


