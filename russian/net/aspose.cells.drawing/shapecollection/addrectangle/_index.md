---
title: "ShapeCollection.AddRectangle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет RectangleShape в лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addrectangle/
---
## ShapeCollection.AddRectangle method

Добавляет RectangleShape на лист.

```csharp
public RectangleShape AddRectangle(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение RectangleShape от её левой строки в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение RectangleShape от его левого столбца, в пикселях. |
| высота | Int32 | Представляет высоту RectangleShape, в пикселях. |
| ширина | Int32 | Представляет ширину RectangleShape, в пикселях. |

### Возвращаемое значение

Объект RectangleShape.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRectangleWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольник, используя указанные параметры
            RectangleShape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Сохраните книгу
            workbook.Save("RectangleShapeDemo.xlsx");
        }
    }
}
```

### См. также

* class [RectangleShape](../../rectangleshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


