---
title: "Shape.IsLockAspectRatio"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. True означает, что соотношение сторон формы заблокировано"
type: docs
url: /ru/net/aspose.cells.drawing/shape/islockaspectratio/
---
## Shape.IsLockAspectRatio property

True означает, что соотношение сторон фигуры заблокировано.

```csharp
[Obsolete("Use Shape.IsAspectRatioLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLockAspectRatio { get; set; }
```

### Примечания

Только для изображений и Ole-объектов. ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство Shape.IsAspectRatioLocked. Это свойство будет удалено через 12 месяцев, начиная с июля 2024 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockAspectRatioDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Заблокировать соотношение сторон
            shape.IsLockAspectRatio = true;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);

            // Разблокировать соотношение сторон
            shape.IsLockAspectRatio = false;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


