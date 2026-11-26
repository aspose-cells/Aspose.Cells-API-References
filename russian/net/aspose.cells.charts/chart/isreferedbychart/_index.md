---
title: "Chart.IsReferedByChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Возвращает, ссылается ли ячейка на диаграмму"
type: docs
url: /ru/net/aspose.cells.charts/chart/isreferedbychart/
---
## Chart.IsReferedByChart method

Возвращает, ссылается ли ячейка на диаграмму.

```csharp
[Obsolete("Use Chart.IsCellReferedByChart(int,int,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsReferedByChart(int rowIndex, int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки |
| columnIndex | Int32 | Индекс столбца |

### Примечания

ПРИМЕЧАНИЕ: Этот метод устарел. Вместо него используйте метод IsCellReferedByChart(int,int,int). Этот метод будет удалён через 12 месяцев, начиная с апреля 2023 года. Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsReferedByChartWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Проверьте, ссылается ли ячейка B2 (строка 1, столбец 1) на диаграмму
                bool isReferred = chart.IsReferedByChart(1, 1);
                
                Console.WriteLine($"Is cell B2 referred by the chart? {isReferred}");
                
                // Проверьте ячейку, которая не находится в диапазоне данных диаграммы
                bool isNotReferred = chart.IsReferedByChart(10, 10);
                Console.WriteLine($"Is cell K11 referred by the chart? {isNotReferred}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsReferedByChart method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("ChartMethodIsReferedByChartWithInt32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


