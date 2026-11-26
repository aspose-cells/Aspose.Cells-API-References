---
title: "ListBox.SelectedIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBox. Получает или задает номер индекса текущего выбранного элемента в list box или combo box. Нумерация с нуля"
type: docs
url: /ru/net/aspose.cells.drawing/listbox/selectedindex/
---
## ListBox.SelectedIndex property

Получает или задает номер индекса текущего выбранного элемента в списке или комбобоксе. Нумерация начинается с нуля.

```csharp
public int SelectedIndex { get; set; }
```

### Примечания

-1 presents no item is selected.

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Item 0");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            
            ListBox listBox = worksheet.Shapes.AddListBox(5, 5, 100, 100, 200, 300);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            listBox.SelectedIndex = 2;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


