---
title: "ShapeCollection.AddArc"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет ArcShape в лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection.AddArc method

Добавляет ArcShape на лист.

```csharp
public ArcShape AddArc(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение ArcShape от его левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение ArcShape от его левого столбца, в пикселях. |
| высота | Int32 | Представляет высоту ArcShape, в пикселях. |
| ширина | Int32 | Представляет ширину ArcShape, в пикселях. |

### Возвращаемое значение

Объект ArcShape.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddArcWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            ArcShape arcShape = shapes.AddArc(10, 10, 100, 50, 45, 180);
            
            workbook.Save("AddArcDemo.xlsx");
        }
    }
}
```

### См. также

* class [ArcShape](../../arcshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


