---
title: "Shape.GetLockedProperty"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Получает значение заблокированного свойства"
type: docs
url: /ru/net/aspose.cells.drawing/shape/getlockedproperty/
---
## Shape.GetLockedProperty method

Получает значение свойства locked.

```csharp
public bool GetLockedProperty(ShapeLockType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | ShapeLockType | Тип заблокированного свойства фигуры. |

### Возвращаемое значение

Возвращает значение заблокированного свойства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLockedPropertyWithShapeLockTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Установить заблокированное свойство для AdjustHandles
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);

            // Проверить, заблокирован ли AdjustHandles
            int noAdjustHandles = 0;
            if (shape.GetLockedProperty(ShapeLockType.AdjustHandles))
                noAdjustHandles = 1;

            Console.WriteLine("AdjustHandles locked status: " + (noAdjustHandles == 1));
        }
    }
}
```

### См. также

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


