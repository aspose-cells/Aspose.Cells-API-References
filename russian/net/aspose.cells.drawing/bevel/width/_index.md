---
title: "Bevel.Width"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Bevel свойство. Получает и задает ширину фаски или насколько глубоко она применяется к фигуре. В единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/bevel/width/
---
## Bevel.Width property

Получает и задает ширину фаски, или насколько она проникает в фигуру. В единицах точек.

```csharp
public double Width { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить первую серию и установить 3D-формат
            Series series = chart.NSeries[0];
            Format3D format3D = series.ShapeProperties.Format3D;
            
            // Настроить свойства фаски с демонстрацией Width
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 12; // Demonstrating Width property
            topBevel.Height = 6;

            // Сохраните книгу
            workbook.Save("BevelWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


