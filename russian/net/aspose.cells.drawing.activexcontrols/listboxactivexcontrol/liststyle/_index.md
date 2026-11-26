---
title: "ListBoxActiveXControl.ListStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBoxActiveXControl. Получает и задает визуальное отображение"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/liststyle/
---
## ListBoxActiveXControl.ListStyle property

Получает и задает визуальное оформление.

```csharp
public ControlListStyle ListStyle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyListStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для list box
            sheet.Cells["A3"].Value = "Sales";
            sheet.Cells["A4"].Value = "Finance";
            sheet.Cells["A5"].Value = "MIS";
            sheet.Cells["A6"].Value = "R&D";
            sheet.Cells["A7"].Value = "Marketing";

            // Добавьте ListBox ActiveX control
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Настройте свойства ListBox
            listBox.ListFillRange = "A3:A7";
            listBox.LinkedCell = "B1";
            listBox.ListStyle = ControlListStyle.Option; // Demonstrating ListStyle property
            listBox.SelectionType = SelectionType.Single;

            // Сохраните книгу
            workbook.Save("ListBoxActiveXControl_ListStyle_Demo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlListStyle](../../controlliststyle/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


