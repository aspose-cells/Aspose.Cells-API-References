---
title: "ThreeDFormat.ExtrusionHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает высоту выдавливания, применяемую к фигуре, в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/extrusionheight/
---
## ThreeDFormat.ExtrusionHeight property

Получает и задает высоту экструдирования, применяемую к фигуре, в единицах точек.

```csharp
public double ExtrusionHeight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyExtrusionHeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец фигуры со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Применить 3D‑форматирование
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionHeight = 32;
            threeDFormat.ContourWidth = 17;
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Проверить сохранённые значения
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;

            Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
            Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
            Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
            Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
            Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


