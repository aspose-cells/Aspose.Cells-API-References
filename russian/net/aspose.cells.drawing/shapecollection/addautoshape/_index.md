---
title: "ShapeCollection.AddAutoShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ShapeCollection метод. Добавляет AutoShape на лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection.AddAutoShape method

Добавляет AutoShape на лист.

```csharp
public Shape AddAutoShape(AutoShapeType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | AutoShapeType | Тип автоформы. |
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
    public class ShapeCollectionMethodAddAutoShapeWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape autoShape = shapes.AddAutoShape(AutoShapeType.Cube, 1, 0, 1, 0, 100, 50);
            
            workbook.Save("AutoShapeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


