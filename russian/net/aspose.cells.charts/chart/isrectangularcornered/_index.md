---
title: "Chart.IsRectangularCornered"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает или задает значение, указывающее, имеет ли область диаграммы прямоугольные углы. По умолчанию true"
type: docs
url: /ru/net/aspose.cells.charts/chart/isrectangularcornered/
---
## Chart.IsRectangularCornered property

Получает или задает значение, указывающее, имеет ли область диаграммы прямоугольные углы. По умолчанию true.

```csharp
public bool IsRectangularCornered { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyIsRectangularCorneredDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Продемонстрировать свойство IsRectangularCornered
            Console.WriteLine("Default IsRectangularCornered: " + chart.IsRectangularCornered);
            
            // Установите значение true, чтобы сделать углы диаграммы прямоугольными
            chart.IsRectangularCornered = true;
            Console.WriteLine("After setting IsRectangularCornered to true: " + chart.IsRectangularCornered);

            // Сохраните книгу
            workbook.Save("ChartPropertyIsRectangularCorneredDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


