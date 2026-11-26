---
title: "GroupShape.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GroupShape. Получает дочернюю фигуру по индексу"
type: docs
url: /ru/net/aspose.cells.drawing/groupshape/item/
---
## GroupShape indexer

Получает дочернюю фигуру по индексу.

```csharp
public Shape this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | индекс дочерней фигуры. |

### Возвращаемое значение

возвращает дочернюю фигуру.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapePropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать две прямоугольные фигуры
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Сгруппировать фигуры
            Shape[] shapesToGroup = new Shape[] { shape1, shape2 };
            GroupShape groupShape = worksheet.Shapes.Group(shapesToGroup);

            // Получить доступ и отобразить свойства первой фигуры
            Shape firstShape = groupShape[0];
            Console.WriteLine($"First shape initial name: {firstShape.Name}");
            Console.WriteLine($"First shape initial text: {firstShape.Text}");

            // Изменить свойства первой фигуры через доступ к Item
            firstShape.Name = "ModifiedRectangle1";
            firstShape.Text = "First Grouped Shape";

            // Получить доступ и изменить вторую фигуру напрямую через индексатор
            groupShape[1].Text = "Second Grouped Shape";

            // Проверьте изменения
            Console.WriteLine($"\nFirst shape updated name: {groupShape[0].Name}");
            Console.WriteLine($"First shape updated text: {groupShape[0].Text}");
            Console.WriteLine($"Second shape updated text: {groupShape[1].Text}");

            // Сохранить изменённую книгу
            workbook.Save("GroupShapePropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


