---
title: "ListBox.SelectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBox. Получает или задает режим выбора указанного list box"
type: docs
url: /ru/net/aspose.cells.drawing/listbox/selectiontype/
---
## ListBox.SelectionType property

Получает или задает режим выбора указанного списка.

```csharp
public SelectionType SelectionType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для list box
            sheet.Cells["A1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Finance");
            sheet.Cells["A3"].PutValue("MIS");
            sheet.Cells["A4"].PutValue("R&D");

            // Добавить list box
            ListBox listBox = sheet.Shapes.AddListBox(1, 0, 2, 0, 100, 80);
            
            // Установить свойства list box
            listBox.InputRange = "A1:A4";
            listBox.LinkedCell = "B1";
            
            // Продемонстрировать свойство SelectionType
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.SelectedIndex = 1; // Select "Finance"

            // Сохраните книгу
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


