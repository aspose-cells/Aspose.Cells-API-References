---
title: "Format3D.HasTopBevelData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Format3D. Указывает, содержит ли фигура данные верхней фаски"
type: docs
url: /ru/net/aspose.cells.drawing/format3d/hastopbeveldata/
---
## Format3D.HasTopBevelData method

Указывает, содержит ли фигура данные о верхней фаске.

```csharp
public bool HasTopBevelData()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class Format3DMethodHasTopBevelDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Создайте 3D‑диаграмму.
            int chartIndex = sheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Получить 3D‑формат
            Format3D format3D = chart.NSeries[0].ShapeProperties.Format3D;

            // Установить верхнюю фаску
            format3D.TopBevel.Type = BevelPresetType.Circle;
            format3D.TopBevel.Width = 6;
            format3D.TopBevel.Height = 6;

            // Проверить и отобразить данные фаски
            if (format3D.HasTopBevelData())
            {
                Console.WriteLine("Top Bevel Type: " + format3D.TopBevel.Type);
                Console.WriteLine("Top Bevel Width: " + format3D.TopBevel.Width);
                Console.WriteLine("Top Bevel Height: " + format3D.TopBevel.Height);
            }

            workbook.Save("Format3DTopBevelDemo.xlsx");
        }
    }
}
```

### См. также

* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


