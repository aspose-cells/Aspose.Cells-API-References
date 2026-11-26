---
title: "ShapeCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Удалить форму"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/removeat/
---
## ShapeCollection.RemoveAt method

Удалить фигуру.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс формы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Добавить первую форму прямоугольника
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Добавить вторую форму прямоугольника
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Удалить первую форму по индексу 0
            shapes.RemoveAt(0);

            // Сохраните книгу
            workbook.Save("ShapeCollectionRemoveAtDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


