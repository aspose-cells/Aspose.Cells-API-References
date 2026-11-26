---
title: "ShapeCollection.AddScrollBar"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет ScrollBar на лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addscrollbar/
---
## ShapeCollection.AddScrollBar method

Добавляет ScrollBar на лист.

```csharp
public ScrollBar AddScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение ScrollBar от его левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение ScrollBar от его левого столбца, в пикселях. |
| высота | Int32 | Представляет высоту ScrollBar, в пикселях. |
| ширина | Int32 | Представляет ширину ScrollBar, в пикселях. |

### Возвращаемое значение

Объект ScrollBar.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddScrollBarWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            ScrollBar scrollBar = shapes.AddScrollBar(1, 0, 100, 20, 0, 100);
            scrollBar.CurrentValue = 50;
            scrollBar.Width = 200;
            scrollBar.Height = 30;

            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### См. также

* class [ScrollBar](../../scrollbar/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


