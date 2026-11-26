---
title: "CheckBoxCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CheckBoxCollection. Добавляет checkBox в коллекцию"
type: docs
url: /ru/net/aspose.cells.drawing/checkboxcollection/add/
---
## CheckBoxCollection.Add method

Добавляет checkBox в коллекцию.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| высота | Int32 | Высота checkBox в пикселях. |
| ширина | Int32 | Ширина checkBox в пикселях. |

### Возвращаемое значение

[`CheckBox`](../../checkbox/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте checkbox, используя параметры Int32 (upperLeftRow, upperLeftColumn, height, width)
            int index = worksheet.CheckBoxes.Add(10, 2, 20, 100);
            
            CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Value = true;
            checkBox.LinkedCell = "B11";
            
            workbook.Save("CheckBoxDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


