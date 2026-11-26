---
title: "ShapeCollection.AddTextBox"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет текстовое поле в рабочий лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

Добавляет текстовое поле на лист.

```csharp
public TextBox AddTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение текстового поля от его верхней строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение текстового поля от его левого столбца, в пикселях. |
| высота | Int32 | Представляет высоту текстового поля, в пикселях. |
| ширина | Int32 | Представляет ширину текстового поля, в пикселях. |

### Возвращаемое значение

Объект [`TextBox`](../../textbox/).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Добавить TextBox с указанными позицией и размером
            TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
            textBox.Text = "Sample TextBox";

            // Сохраните книгу
            workbook.Save("TextBoxDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


