---
title: "ListBoxActiveXControl.BorderStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBoxActiveXControl. Получает и задает тип границы, используемой элементом управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/borderstyle/
---
## ListBoxActiveXControl.BorderStyle property

Получает и задает тип границы, используемой элементом управления.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления ListBox ActiveX с исправленными параметрами
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 
                1, 0, 1, 100, 150, 30); // Added height parameter
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Установить свойство BorderStyle
            listBox.BorderStyle = ControlBorderType.None;

            // Проверить и вывести стиль границы
            Console.WriteLine("BorderStyle: " + listBox.BorderStyle);

            workbook.Save("ListBoxBorderStyleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlBorderType](../../controlbordertype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


