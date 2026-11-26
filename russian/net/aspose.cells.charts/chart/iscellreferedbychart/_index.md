---
title: "Chart.IsCellReferedByChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Возвращает, относится ли ячейка к диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/chart/iscellreferedbychart/
---
## Chart.IsCellReferedByChart method

Возвращает, относится ли ячейка к диаграмме.

```csharp
public bool IsCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | Индекс листа -1 означает лист, содержащий текущую диаграмму. |
| rowIndex | Int32 | Индекс строки |
| columnIndex | Int32 | Индекс столбца |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodIsCellReferedByChartWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Проверьте, ссылается ли ячейка на диаграмму
            bool isReferred = chart.IsCellReferedByChart(0, 1, 0); // Check if B2 is referred
            Console.WriteLine("Is cell B2 referred by chart: " + isReferred);
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


