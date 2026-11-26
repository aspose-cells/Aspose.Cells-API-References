---
title: "ChartPointCollection.GetEnumerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ChartPointCollection method. Возвращает перечислитель для всей ChartPointCollection"
type: docs
url: /ru/net/aspose.cells.charts/chartpointcollection/getenumerator/
---
## ChartPointCollection.GetEnumerator method

Возвращает перечислитель для всей [`ChartPointCollection`](../).

```csharp
public IEnumerator GetEnumerator()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Collections;

    public class ChartPointCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Получить коллекцию точек первой серии
                ChartPointCollection points = chart.NSeries[0].Points;

                // Вызовите метод GetEnumerator
                IEnumerator enumerator = points.GetEnumerator();

                Console.WriteLine("Iterating through chart points:");
                while (enumerator.MoveNext())
                {
                    ChartPoint point = (ChartPoint)enumerator.Current;
                    Console.WriteLine($"Point value: {point.YValue}");
                }

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


