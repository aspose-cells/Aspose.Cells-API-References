---
title: "ShapeCollection.AddListBox"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ShapeCollection метод. Добавляет ListBox на лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addlistbox/
---
## ShapeCollection.AddListBox method

Добавляет ListBox на лист.

```csharp
public ListBox AddListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение ListBox от его левой строки, в единицах пикселей. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение ListBox от его левого столбца, в единицах пикселей. |
| высота | Int32 | Представляет высоту ListBox, в единицах пикселей. |
| ширина | Int32 | Представляет ширину ListBox, в единицах пикселей. |

### Возвращаемое значение

Объект ListBox.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddListBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить список в лист
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 50);

            // Добавить элементы в список
            listBox.SetInputRange("A1:A3", false, false);
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Сохраните книгу
            workbook.Save("ListBoxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListBox](../../listbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


