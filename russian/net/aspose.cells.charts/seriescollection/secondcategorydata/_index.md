---
title: "SeriesCollection.SecondCategoryData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SeriesCollection. Получает или задает диапазон значений второй оси категорий. Это может быть диапазон ячеек, например d1e10, или последовательность значений, например 26810. Действует только когда некоторые ряды построены на второй оси."
type: docs
url: /ru/net/aspose.cells.charts/seriescollection/secondcategorydata/
---
## SeriesCollection.SecondCategoryData property

Получает или задает диапазон значений второй оси категорий. Это может быть диапазон ячеек (например, "d1:e10"), или последовательность значений (например, "{2,6,8,10}"). Действует только когда некоторые серии построены на второй оси.

```csharp
public string SecondCategoryData { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertySecondCategoryDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Primary Categories");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Secondary Categories");
            worksheet.Cells["B2"].PutValue("SubCat1");
            worksheet.Cells["B3"].PutValue("SubCat2");
            worksheet.Cells["B4"].PutValue("SubCat3");
            
            worksheet.Cells["C1"].PutValue("Values");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);
            worksheet.Cells["C4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить данные серии
            chart.NSeries.Add("C2:C4", true);
            
            // Установить данные основной категории
            chart.NSeries.CategoryData = "A2:A4";
            
            // Установить данные вторичной категории
            chart.NSeries.SecondCategoryData = "B2:B4";

            // Сохраните книгу
            workbook.Save("SecondCategoryDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


