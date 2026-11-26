---
title: "Shape.IsSameSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Возвращает, одинаковая ли форма"
type: docs
url: /ru/net/aspose.cells.drawing/shape/issamesetting/
---
## Shape.IsSameSetting method

Возвращает, одинаковы ли формы.

```csharp
public virtual bool IsSameSetting(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object |  |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodIsSameSettingWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape1 = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            if (shape1.IsSameSetting(shape1))
            {
                Console.WriteLine("Same shape object - settings match.");
            }

            if (!shape1.IsSameSetting(shape2))
            {
                Console.WriteLine("Different shape objects - settings don't match.");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


