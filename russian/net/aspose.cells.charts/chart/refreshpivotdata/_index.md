---
title: "Chart.RefreshPivotData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Обновляет данные диаграммы из сводной таблицы"
type: docs
url: /ru/net/aspose.cells.charts/chart/refreshpivotdata/
---
## Chart.RefreshPivotData method

Обновляет данные диаграммы из сводной таблицы.

```csharp
public void RefreshPivotData()
```

### Примечания

Мы соберём данные из источника сводных данных в отчёт сводной таблицы. Этот метод используется только для сбора всех данных в сводную диаграмму.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodRefreshPivotDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные в первый лист
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(100);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(200);
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B4"].PutValue(300);

            // Создайте сводную таблицу
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            pivotSheet.PivotTables.Add("A1", dataSheet.Cells["A1:B4"].Name, "PivotTable1");

            // Добавьте диаграмму
            int chartIndex = pivotSheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Aspose.Cells.Charts.Chart chart = pivotSheet.Charts[chartIndex];
            
            // Установить источник данных сводной диаграммы
            chart.PivotSource = "Pivot!PivotTable1";
            
            // Обновить данные сводной диаграммы
            chart.RefreshPivotData();
            
            // Сохраните книгу
            workbook.Save("PivotChartWithRefresh.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


