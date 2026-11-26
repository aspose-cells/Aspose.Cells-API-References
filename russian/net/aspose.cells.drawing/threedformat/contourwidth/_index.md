---
title: "ThreeDFormat.ContourWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает ширину контура фигуры в единицах пунктов"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/contourwidth/
---
## ThreeDFormat.ContourWidth property

Получает и задает ширину контура фигуры, в единицах точек.

```csharp
public double ContourWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyContourWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Добавьте форму на лист со всеми необходимыми параметрами
            Shape sh = ws.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);

            // Применить 3D‑форматирование
            ThreeDFormat n3df = sh.ThreeDFormat;
            n3df.ContourWidth = 17;
            n3df.ExtrusionHeight = 32;
            n3df.TopBevelType = (BevelType)BevelPresetType.HardEdge;

            // Сохраните книгу
            wb.Save("output.xlsx");

            // Проверить сохранённые значения
            Workbook wb2 = new Workbook("output.xlsx");
            Shape sh2 = wb2.Worksheets[0].Shapes[0];
            ThreeDFormat n3df2 = sh2.ThreeDFormat;

            Console.WriteLine("ContourWidth: " + n3df2.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + n3df2.ExtrusionHeight);
            Console.WriteLine("TopBevelType: " + n3df2.TopBevelType);
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


