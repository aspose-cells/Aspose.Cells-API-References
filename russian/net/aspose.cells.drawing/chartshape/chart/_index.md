---
title: "ChartShape.Chart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartShape. Возвращает объект Chart, который представляет диаграмму, содержащуюся в объекте"
type: docs
url: /ru/net/aspose.cells.drawing/chartshape/chart/
---
## ChartShape.Chart property

Возвращает объект Chart, представляющий диаграмму, содержащуюся в объекте.

```csharp
public Chart Chart { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartShapePropertyChartDemo
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
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить экземпляр ChartShape
            ChartShape chartShape = (ChartShape)chart.ChartObject;

            // Получить доступ к свойству Chart (только для чтения)
            Chart accessedChart = chartShape.Chart;

            // Отобразить свойства диаграммы
            Console.WriteLine("Chart Name: " + accessedChart.Name);
            Console.WriteLine("Chart Type: " + accessedChart.Type);
            Console.WriteLine("Show Legend: " + accessedChart.ShowLegend);

            // Изменить свойства диаграммы через объект Chart
            accessedChart.Name = "Sales Chart";
            accessedChart.ShowLegend = false;
            accessedChart.Title.Text = "Product Sales Distribution";

            // Изменить тип диаграммы
            accessedChart.Type = ChartType.Pie;

            // Сохранить результат
            workbook.Save("ChartShapePropertyChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../../../aspose.cells.charts/chart/)
* class [ChartShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


