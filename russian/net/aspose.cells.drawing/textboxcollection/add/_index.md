---
title: "TextBoxCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TextBoxCollection. Добавляет текстовое поле в коллекцию"
type: docs
url: /ru/net/aspose.cells.drawing/textboxcollection/add/
---
## TextBoxCollection.Add method

Добавляет текстовое поле в коллекцию.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| высота | Int32 | Высота textbox, в пикселях. |
| ширина | Int32 | Ширина textbox, в пикселях. |

### Возвращаемое значение

[`TextBox`](../../textbox/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int index = worksheet.TextBoxes.Add(1, 1, 50, 100);
            Console.WriteLine("TextBox added at index: " + index);
        }
    }
}
```

### См. также

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


