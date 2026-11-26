---
title: "Перечисление SelectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.SelectionType. Тип выбора списка"
type: docs
url: /ru/net/aspose.cells.drawing/selectiontype/
---
## SelectionType enumeration

Тип выбора списка.

```csharp
public enum SelectionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Single | `0` | Тип одиночного выбора. |
| Multi | `1` | Тип множественного выбора. |
| Extend | `2` | Тип расширенного выбора. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassSelectionTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить список в лист
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 5, 10);

            // Установить тип выбора в Single
            listBox.SelectionType = SelectionType.Single;

            // Добавить элементы в список
            listBox.SetInputRange("A1:A5", false, false);

            // Проверить тип выбора
            Console.WriteLine("ListBox SelectionType: " + listBox.SelectionType);

            // Сохраните книгу
            workbook.Save("SelectionTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


