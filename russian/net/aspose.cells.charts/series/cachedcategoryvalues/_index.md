---
title: "Series.CachedCategoryValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Возвращает кэшированные значения категорий для серии"
type: docs
url: /ru/net/aspose.cells.charts/series/cachedcategoryvalues/
---
## Series.CachedCategoryValues property

Возвращает кэшированные значения категорий для серии

```csharp
[Obsolete("internal use only")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList CachedCategoryValues { get; }
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

    public class SeriesPropertyCachedCategoryValuesDemo
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

                // Отобразить кэшированные значения категорий
                ArrayList cachedCategoryValues = series.CachedCategoryValues;
                Console.WriteLine("CachedCategoryValues count: " + cachedCategoryValues.Count);

                // Отобразить каждое кэшированное значение категории
                for (int i = 0; i < cachedCategoryValues.Count; i++)
                {
                    Console.WriteLine("Cached Category Value " + (i + 1) + ": " + cachedCategoryValues[i]);
                }

                // Сохраните книгу
                workbook.Save("CachedCategoryValuesDemo.xlsx");
                Console.WriteLine("CachedCategoryValues demonstration completed successfully.");
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


