---
title: "ThreeDFormat.TopBevelWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает ширину верхней фаски или насколько глубоко она применяется к фигуре. В единицах пунктов"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/topbevelwidth/
---
## ThreeDFormat.TopBevelWidth property

Получает и задает ширину верхней фаски, или насколько глубоко она применяется к фигуре. В единицах точек.

```csharp
public double TopBevelWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму в лист с правильными параметрами
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 0, 0);

            // Получить 3D-формат фигуры
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Установить 3D‑свойства, включая TopBevelWidth
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;
            threeDFormat.ContourWidth = 17;
            threeDFormat.ExtrusionHeight = 32;

            // Сохраните книгу
            workbook.Save("ThreeDFormatDemo.xlsx");

            // Проверить сохранённые свойства
            Workbook loadedWorkbook = new Workbook("ThreeDFormatDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;

            Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
            Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
            Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
            Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


