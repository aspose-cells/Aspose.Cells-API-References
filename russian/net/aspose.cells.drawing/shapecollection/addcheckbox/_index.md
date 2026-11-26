---
title: "ShapeCollection.AddCheckBox"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет флажок в лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addcheckbox/
---
## ShapeCollection.AddCheckBox method

Добавляет флажок на лист.

```csharp
public CheckBox AddCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение checkbox от его верхней строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение текстового поля от его левого столбца, в пикселях. |
| высота | Int32 | Высота textbox, в пикселях. |
| ширина | Int32 | Ширина textbox, в пикселях. |

### Возвращаемое значение

Индекс нового объекта CheckBox.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCheckBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Добавить CheckBox, используя указанные параметры
            Aspose.Cells.Drawing.CheckBox checkBox = shapes.AddCheckBox(1, 0, 1, 0, 100, 50);

            // Сохраните книгу
            workbook.Save("CheckBoxDemo.xlsx");
        }
    }
}
```

### См. также

* class [CheckBox](../../checkbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


