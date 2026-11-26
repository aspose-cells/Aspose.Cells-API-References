---
title: "ShapeCollection.AddComboBox"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет ComboBox на лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addcombobox/
---
## ShapeCollection.AddComboBox method

Добавляет ComboBox на лист.

```csharp
public ComboBox AddComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение ComboBox от его левой строки, в единицах пикселей. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение ComboBox от его левого столбца, в единицах пикселей. |
| высота | Int32 | Представляет высоту ComboBox, в единицах пикселей. |
| ширина | Int32 | Представляет ширину ComboBox, в единицах пикселей. |

### Возвращаемое значение

Объект ComboBox.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddComboBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Добавьте комбобокс с указанными параметрами
            Aspose.Cells.Drawing.ComboBox comboBox = shapes.AddComboBox(1, 0, 1, 0, 100, 50);

            // Добавьте элементы в комбобокс, задав значения ячеек
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Установите диапазон ввода для combo box
            comboBox.InputRange = "A1:A3";
            comboBox.DropDownLines = 3;

            // Сохраните книгу
            workbook.Save("AddComboBoxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBox](../../combobox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


