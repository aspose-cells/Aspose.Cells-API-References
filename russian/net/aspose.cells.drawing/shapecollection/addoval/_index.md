---
title: "ShapeCollection.AddOval"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ShapeCollection метод. Добавляет Oval на лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addoval/
---
## ShapeCollection.AddOval method

Добавляет овал на лист.

```csharp
public Oval AddOval(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение Oval от его левой строки, в единицах пикселей. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение Oval от его левого столбца, в единицах пикселей. |
| высота | Int32 | Представляет высоту Oval, в единицах пикселей. |
| ширина | Int32 | Представляет ширину Oval, в единицах пикселей. |

### Возвращаемое значение

Объект Oval.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddOvalWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить овальную форму на лист
            ShapeCollection shapes = worksheet.Shapes;
            Oval oval = shapes.AddOval(1, 0, 1, 0, 50, 50);

            // Сохраните книгу
            workbook.Save("AddOvalDemo.xlsx");
        }
    }
}
```

### См. также

* class [Oval](../../oval/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


