---
title: "Shape.AnchorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает тип заполнителя привязки формы"
type: docs
url: /ru/net/aspose.cells.drawing/shape/anchortype/
---
## Shape.AnchorType property

Получает и задает тип заполнителя привязки фигуры.

```csharp
public ShapeAnchorType AnchorType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму с типом привязки по умолчанию
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            
            // Проверьте и измените тип привязки
            if (shape.AnchorType == ShapeAnchorType.OneCellAnchor)
            {
                shape.AnchorType = ShapeAnchorType.TwoCellAnchor;
                Console.WriteLine("Anchor type changed to TwoCellAnchor");
            }
            
            // Сохраните книгу
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ShapeAnchorType](../../shapeanchortype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


