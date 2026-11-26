---
title: "Shape.AlignTopRightCorner"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Перемещает изображение в правый верхний угол"
type: docs
url: /ru/net/aspose.cells.drawing/shape/aligntoprightcorner/
---
## Shape.AlignTopRightCorner method

Перемещает изображение в правый верхний угол.

```csharp
public void AlignTopRightCorner(int topRow, int rightColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | индекс строки. |
| rightColumn | Int32 | индекс столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAlignTopRightCornerWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец формы для выравнивания
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Выровняйте правый верхний угол формы по строке 2, столбцу 5
            shape.AlignTopRightCorner(2, 5);

            // Сохраните книгу
            workbook.Save("AlignTopRightCornerDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


