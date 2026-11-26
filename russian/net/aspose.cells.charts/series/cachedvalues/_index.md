---
title: "Series.CachedValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает кэшированные значения для серии"
type: docs
url: /ru/net/aspose.cells.charts/series/cachedvalues/
---
## Series.CachedValues property

Получает кэшированные значения для серии

```csharp
[Obsolete("internal use only")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList CachedValues { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство в настоящее время предназначено только для внутреннего использования. Оно будет изменено или удалено в следующей версии.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Collections;

    public class SeriesPropertyCachedValuesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Получить доступ к первой серии
                Series series = chart.NSeries[0];

                // Отобразить кэшированные значения
                ArrayList cachedValues = series.CachedValues;
                Console.WriteLine("CachedValues count: " + cachedValues.Count);

                // Отобразить каждое кэшированное значение
                for (int i = 0; i < cachedValues.Count; i++)
                {
                    Console.WriteLine("Cached Value " + (i + 1) + ": " + cachedValues[i]);
                }

                // Сохраните книгу
                workbook.Save("CachedValuesDemo.xlsx");
                Console.WriteLine("CachedValues demonstration completed successfully.");
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


