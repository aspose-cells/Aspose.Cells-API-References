---
title: "Bevel.Height"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Bevel свойство. Получает и задает высоту фаски или насколько она поднимается над фигурой. В единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/bevel/height/
---
## Bevel.Height property

Получает и задает высоту фаски, или насколько она расположена над фигурой. В единицах точек.

```csharp
public double Height { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class BevelPropertyHeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(1500);

            // Добавить 3D столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Получить доступ к 3D-формату области построения
            Format3D format3D = chart.PlotArea.ShapeProperties.Format3D;

            // Настроить верхнюю фаску с помощью свойства Height
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.ArtDeco;
            topBevel.Width = 8;
            topBevel.Height = 4.5; // Demonstrating Height property usage

            // Сохраните книгу
            workbook.Save("BevelHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


