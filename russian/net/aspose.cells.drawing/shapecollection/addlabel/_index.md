---
title: "ShapeCollection.AddLabel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет Label в лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

Добавляет метку на лист.

```csharp
public Label AddLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение Label от его левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение Label от его левого столбца, в пикселях. |
| высота | Int32 | Представляет высоту Label, в пикселях. |
| ширина | Int32 | Представляет ширину Label, в пикселях. |

### Возвращаемое значение

Объект Label.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLabelWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Добавить метку в лист
            Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
            label.Text = "Sample Label";

            // Сохраните книгу
            workbook.Save("AddLabelDemo.xlsx");
        }
    }
}
```

### См. также

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


