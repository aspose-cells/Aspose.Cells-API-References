---
title: "ShapeCollection.AddGroupBox"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет GroupBox на лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

Добавляет GroupBox на лист.

```csharp
public GroupBox AddGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение GroupBox от её левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение GroupBox от её левой колонки, в пикселях. |
| высота | Int32 | Представляет высоту GroupBox, в пикселях. |
| ширина | Int32 | Представляет ширину GroupBox, в пикселях. |

### Возвращаемое значение

Объект GroupBox.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddGroupBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить GroupBox на лист
            ShapeCollection shapes = worksheet.Shapes;
            Aspose.Cells.Drawing.GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);

            // Сохраните книгу
            workbook.Save("GroupBoxDemo.xlsx");
        }
    }
}
```

### См. также

* class [GroupBox](../../groupbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


