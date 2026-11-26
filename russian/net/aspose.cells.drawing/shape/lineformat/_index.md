---
title: "Shape.LineFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Возвращает объект MsoLineFormat, содержащий свойства форматирования линий для указанной фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

Возвращает объект MsoLineFormat, содержащий свойства форматирования линий для указанной фигуры.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Line. Это свойство будет удалено через 12 месяцев, начиная с июля 2016 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить прямоугольную форму на первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
            
            // Установите свойства формы
            rectangle.Placement = PlacementType.FreeFloating;
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            
            // Продемонстрировать использование LineFormat
            rectangle.LineFormat.Weight = 3; // Set line weight
            rectangle.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            rectangle.Line.SolidFill.Color = System.Drawing.Color.DarkBlue; // Correct way to set line color
            
            // Сохраните книгу
            workbook.Save("ShapeLineFormatDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


