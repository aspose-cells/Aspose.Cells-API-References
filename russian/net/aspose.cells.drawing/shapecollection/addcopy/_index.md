---
title: "ShapeCollection.AddCopy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет и копирует форму на лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addcopy/
---
## AddCopy(Shape, int, int, int, int) {#addcopy}

Добавляет и копирует фигуру на лист.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceShape | Фигура | Исходная фигура. |
| topRow | Int32 | Индекс верхней строки. |
| верх | Int32 | Представляет вертикальное смещение от его верхней строки, в пикселях. |
| leftColumn | Int32 | Индекс левой колонки. |
| влево | Int32 | Представляет горизонтальное смещение от его левого столбца, в пикселях. |

### Возвращаемое значение

Новый объект [`Shape`](../../shape/).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCopyWithShapeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Добавить прямоугольную фигуру
            RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Добавить копию прямоугольной фигуры с новой позицией
            shapes.AddCopy(rectangle, 7, 0, 7, 0);

            // Сохраните книгу
            workbook.Save("ShapeCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Shape, int, int, int, int, CopyOptions) {#addcopy_1}

Добавляет и копирует фигуру на лист.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, 
    CopyOptions copyOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceShape | Фигура | Исходная фигура. |
| topRow | Int32 | Индекс верхней строки. |
| верх | Int32 | Представляет вертикальное смещение от его верхней строки, в пикселях. |
| leftColumn | Int32 | Индекс левой колонки. |
| влево | Int32 | Представляет горизонтальное смещение от его левого столбца, в пикселях. |
| copyOptions | CopyOptions | Параметры копирования фигур. |

### Возвращаемое значение

Новый объект [`Shape`](../../shape/).

### Примеры

```csharp

[C#]
//добавить фигуру
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//Добавляет и копирует фигуру.
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

### См. также

* class [Shape](../../shape/)
* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


