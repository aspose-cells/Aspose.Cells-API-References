---
title: "TextBoxActiveXControl.IsMultiLine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Указывает, может ли элемент управления отображать более одной строки текста"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/ismultiline/
---
## TextBoxActiveXControl.IsMultiLine property

Указывает, может ли элемент управления отображать более одной строки текста.

```csharp
public bool IsMultiLine { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsMultiLineDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления TextBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 200, 100, 0, 0);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Продемонстрируйте свойство IsMultiLine
            if (!textBox.IsMultiLine)
            {
                textBox.IsMultiLine = true;
                textBox.Text = "This is a multi-line text box.\nSecond line of text.";
            }

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlIsMultiLineDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


