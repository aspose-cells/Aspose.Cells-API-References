---
title: "ListBoxActiveXControl.ShowColumnHeads"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBoxActiveXControl. Указывает, отображаются ли заголовки столбцов"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/showcolumnheads/
---
## ListBoxActiveXControl.ShowColumnHeads property

Указывает, отображаются ли заголовки столбцов.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления ListBox ActiveX со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ListBox, 
                1, 1, 100, 100,  // Left, Top, Width, Height
                0, 0);           // UpperLeftRow, UpperLeftColumn

            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Установить свойства для ListBox
            listBox.ColumnCount = 2;
            listBox.ListWidth = 150;
            listBox.ShowColumnHeads = true; // Demonstrate ShowColumnHeads property

            // Добавьте некоторые образцы данных.
            listBox.Value = "Header1\tHeader2\nItem1\tData1\nItem2\tData2";

            // Сохраните книгу
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


