---
title: "TextBoxActiveXControl.IsEditable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Указывает, может ли пользователь вводить текст в элемент управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iseditable/
---
## TextBoxActiveXControl.IsEditable property

Указывает, может ли пользователь вводить текст в элемент управления.

```csharp
public bool IsEditable { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsEditableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления TextBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Продемонстрируйте свойство IsEditable
            Console.WriteLine("Initial IsEditable: " + textBox.IsEditable);
            
            // Переключите свойство IsEditable
            textBox.IsEditable = !textBox.IsEditable;
            Console.WriteLine("After toggle IsEditable: " + textBox.IsEditable);

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


