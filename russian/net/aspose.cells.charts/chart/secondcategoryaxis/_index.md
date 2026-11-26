---
title: "Chart.SecondCategoryAxis"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает вторую ось X диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/secondcategoryaxis/
---
## Chart.SecondCategoryAxis property

Получает вторую ось X диаграммы.

```csharp
public Axis SecondCategoryAxis { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySecondCategoryAxisDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Добавить диаграмму со вторичной осью
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию к диаграмме
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Включить вторичную ось категорий
            chart.SecondCategoryAxis.IsVisible = true;
            chart.SecondCategoryAxis.Title.Text = "Secondary Category Axis";
            
            // Установить некоторые свойства вторичной оси категорий
            chart.SecondCategoryAxis.MajorTickMark = TickMarkType.Cross;
            chart.SecondCategoryAxis.MinorTickMark = TickMarkType.Outside;
            chart.SecondCategoryAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;

            // Сохраните книгу
            workbook.Save("SecondCategoryAxisDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


