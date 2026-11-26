---
title: "ShapeCollection.AddShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет Shape в рабочий лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addshape/
---
## ShapeCollection.AddShape method

Добавляет форму на лист.

```csharp
public Shape AddShape(MsoDrawingType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | MsoDrawingType | Тип рисования Mso. |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение Shape от его левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение Shape от его левого столбца, в пикселях. |
| высота | Int32 | Представляет высоту Shape, в пикселях. |
| ширина | Int32 | Представляет ширину Shape, в пикселях. |

### Возвращаемое значение

Объект Shape.

### Примечания

Тип не может быть Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 200, 50);
            
            Console.WriteLine("Shape added successfully.");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


