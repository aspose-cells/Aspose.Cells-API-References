---
title: "Series.DisplayName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает имя серии, которое отображается на графике диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/series/displayname/
---
## Series.DisplayName property

Получает имя серии, отображаемое на графике диаграммы.

```csharp
public string DisplayName { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesPropertyDisplayNameDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Получить доступ к первой серии и отобразить её DisplayName
                Series series = chart.NSeries[0];
                Console.WriteLine("Series DisplayName: " + series.DisplayName);

                // Также показать свойство Name для сравнения
                Console.WriteLine("Series Name: " + series.Name);

                // Сохраните книгу
                workbook.Save("DisplayNameDemo.xlsx");
                Console.WriteLine("DisplayName has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


