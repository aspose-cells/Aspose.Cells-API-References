---
title: "TextBoxActiveXControl.BorderStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Получает и задает тип границы, используемой элементом управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderstyle/
---
## TextBoxActiveXControl.BorderStyle property

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
    public class TextBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить ActiveX‑элемент TextBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 100, 100, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Задайте свойство BorderStyle
            textBox.BorderStyle = ControlBorderType.Single;

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlBorderType](../../controlbordertype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


