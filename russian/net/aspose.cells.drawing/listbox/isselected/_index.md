---
title: "ListBox.IsSelected"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListBox. Указывает, выбран ли элемент"
type: docs
url: /ru/net/aspose.cells.drawing/listbox/isselected/
---
## ListBox.IsSelected method

Указывает, выбран ли элемент.

```csharp
public bool IsSelected(int itemIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| itemIndex | Int32 | Индекс элемента. |

### Возвращаемое значение

выбран ли элемент.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxMethodIsSelectedWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить список в лист
            ListBox listBox = worksheet.Shapes.AddListBox(0, 0, 100, 100, 200, 200);

            // Установить элементы списка через связанный диапазон ячеек
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            listBox.LinkedCell = "A1:A3";

            // Выберите элемент
            listBox.SelectedIndex = 0;

            // Проверьте статус выбора, используя IsSelected с параметром Int32
            Console.WriteLine("Item 0 selected: " + listBox.IsSelected(0));
            Console.WriteLine("Item 1 selected: " + listBox.IsSelected(1));
            Console.WriteLine("Item 2 selected: " + listBox.IsSelected(2));
        }
    }
}
```

### См. также

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


