---
title: "ShapeCollection.AddButton"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет кнопку Button в лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addbutton/
---
## ShapeCollection.AddButton method

Добавляет кнопку на лист.

```csharp
public Button AddButton(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение Button от его левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение Button от его левого столбца, в пикселях. |
| высота | Int32 | Представляет высоту Button, в пикселях. |
| ширина | Int32 | Представляет ширину Button, в пикселях. |

### Возвращаемое значение

Объект Button.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте кнопку, используя указанные параметры
            Aspose.Cells.Drawing.Button button = worksheet.Shapes.AddButton(1, 0, 1, 0, 100, 50);
            button.Text = "Click Me";

            // Сохраните книгу
            workbook.Save("ButtonDemo.xlsx");
        }
    }
}
```

### См. также

* class [Button](../../button/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


