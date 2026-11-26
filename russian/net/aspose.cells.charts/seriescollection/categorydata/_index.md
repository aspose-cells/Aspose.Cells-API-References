---
title: "SeriesCollection.CategoryData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SeriesCollection. Получает или задает диапазон значений оси категорий. Это может быть диапазон ячеек, например d1e10, или последовательность значений, например 26810"
type: docs
url: /ru/net/aspose.cells.charts/seriescollection/categorydata/
---
## SeriesCollection.CategoryData property

Получает или задает диапазон значений оси категорий. Это может быть диапазон ячеек (например, "d1:e10") или последовательность значений (например, "{2,6,8,10}").

```csharp
public string CategoryData { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyCategoryDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("=Sheet1!$B$2:$B$10", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$10";
            
            // Сохраните книгу
            workbook.Save("CategoryDataDemo.xlsx");
            
            // Проверьте свойство CategoryData
            Console.WriteLine("Chart CategoryData: " + chart.NSeries.CategoryData);
        }
    }
}
```

### См. также

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


