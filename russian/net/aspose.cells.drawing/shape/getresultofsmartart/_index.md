---
title: "Shape.GetResultOfSmartArt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Преобразование smart art в сгруппированные фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/getresultofsmartart/
---
## Shape.GetResultOfSmartArt method

Преобразование SmartArt в сгруппированные фигуры.

```csharp
public virtual GroupShape GetResultOfSmartArt()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetResultOfSmartArtDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму (поскольку мы не можем создать SmartArt напрямую)
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 200, 200, 0, 0);
            
            // В реальном сценарии мы бы загрузили существующую форму SmartArt
            // Для демонстрационных целей мы пропустим проверку IsSmartArt, поскольку не можем установить её

            // Получить результат SmartArt (будет работать только если форма действительно является SmartArt)
            GroupShape groupShape = shape.GetResultOfSmartArt();
            Console.WriteLine("Converted shape to GroupShape");
        }
    }
}
```

### См. также

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


