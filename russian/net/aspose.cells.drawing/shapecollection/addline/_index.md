---
title: "ShapeCollection.AddLine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет LineShape в лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addline/
---
## ShapeCollection.AddLine method

Добавляет LineShape на лист.

```csharp
public LineShape AddLine(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение LineShape от его левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение LineShape от его левого столбца, в пикселях. |
| высота | Int32 | Представляет высоту LineShape, в пикселях. |
| ширина | Int32 | Представляет ширину LineShape, в пикселях. |

### Возвращаемое значение

Объект LineShape.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLineWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            LineShape lineShape = shapes.AddLine(1, 0, 1, 0, 100, 50);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [LineShape](../../lineshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


