---
title: "Chart.Move"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Перемещает диаграмму в указанное место"
type: docs
url: /ru/net/aspose.cells.charts/chart/move/
---
## Chart.Move method

Перемещает диаграмму в указанное место.

```csharp
public void Move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| rightColumn | Int32 | Индекс столбца нижнего правого угла |
| bottomRow | Int32 | Индекс строки нижнего правого угла |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodMoveWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Исходное положение диаграммы
                Console.WriteLine($"Original position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Переместить диаграмму в новое положение (строки 10-20, столбцы 2-8)
                chart.Move(10, 2, 20, 8);

                // Отобразить новое положение
                Console.WriteLine($"New position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Сохраните книгу
                workbook.Save("ChartMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


