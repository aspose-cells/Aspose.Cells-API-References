---
title: "ListBox.PageChange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBox. Указывает величину, на которую изменяется значение управления, когда пользователь нажимает область прокрутки «страница вверх» или «страница вниз»"
type: docs
url: /ru/net/aspose.cells.drawing/listbox/pagechange/
---
## ListBox.PageChange property

Указывает величину, на которую изменяется значение элемента управления, когда пользователь нажимает область прокрутки «страница вверх» или «страница вниз».

```csharp
public int PageChange { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyPageChangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму ListBox
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 100);

            // Установить несколько элементов для ListBox
            listBox.SetInputRange("A1:A5", false, false);
            
            // Установить свойство PageChange
            listBox.PageChange = 2;

            // Сохраните книгу
            workbook.Save("ListBoxPageChangeDemo.xlsx");

            // Отобразить значение PageChange
            Console.WriteLine("ListBox PageChange value: " + listBox.PageChange);
        }
    }
}
```

### См. также

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


