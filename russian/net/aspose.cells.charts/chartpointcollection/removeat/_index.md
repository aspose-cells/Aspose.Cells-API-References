---
title: "ChartPointCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartPointCollection. Удаляет точку по индексу серии"
type: docs
url: /ru/net/aspose.cells.charts/chartpointcollection/removeat/
---
## ChartPointCollection.RemoveAt method

Удаляет точку по индексу серии.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс точки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionMethodRemoveAtWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить коллекцию точек первой серии
            ChartPointCollection points = chart.NSeries[0].Points;

            try
            {
                // Отобразить начальное количество
                Console.WriteLine($"Initial points count: {points.Count}");

                // Удалить точку с индексом 1 (вторая точка)
                points.RemoveAt(1);

                // Отобразить результат
                Console.WriteLine($"Points count after RemoveAt: {points.Count}");
                Console.WriteLine("Point at index 1 removed successfully.");

                // Сохраните книгу
                workbook.Save("ChartPointCollectionRemoveAtDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


