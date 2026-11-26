---
title: "Shape.HeightScale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает масштаб высоты в процентах от оригинальной высоты изображения. Если фигура не является изображением, свойство HeightScale возвращает только 100"
type: docs
url: /ru/net/aspose.cells.drawing/shape/heightscale/
---
## Shape.HeightScale property

Получает и задает масштаб высоты в процентах от исходной высоты изображения. Если фигура не является изображением, свойство HeightScale возвращает только 100;

```csharp
public int HeightScale { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightScaleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 150);

            // Установить начальный масштаб высоты
            shape.HeightScale = 50;
            Console.WriteLine("Initial HeightScale: " + shape.HeightScale);

            // Изменить масштаб высоты, если условие выполнено
            if (shape.HeightScale == 50)
            {
                shape.HeightScale = 75;
                Console.WriteLine("Modified HeightScale: " + shape.HeightScale);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


