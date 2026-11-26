---
title: "Shape.SetLockedProperty"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Устанавливает заблокированное свойство"
type: docs
url: /ru/net/aspose.cells.drawing/shape/setlockedproperty/
---
## Shape.SetLockedProperty method

Задать свойство locked.

```csharp
public void SetLockedProperty(ShapeLockType type, bool value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | ShapeLockType | Тип блокировки. |
| значение | Boolean | Значение свойства. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLockedPropertyWithShapeLockTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец фигуры со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Продемонстрируйте использование SetLockedProperty
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);
            shape.SetLockedProperty(ShapeLockType.Selection, false);

            Console.WriteLine("Shape locked properties set successfully.");
        }
    }
}
```

### См. также

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


