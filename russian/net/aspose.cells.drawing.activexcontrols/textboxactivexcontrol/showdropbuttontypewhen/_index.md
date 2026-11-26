---
title: "TextBoxActiveXControl.ShowDropButtonTypeWhen"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Указывает символ, отображаемый на кнопке раскрытия"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen/
---
## TextBoxActiveXControl.ShowDropButtonTypeWhen property

Указывает символ, отображаемый на кнопке раскрытия

```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyShowDropButtonTypeWhenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить ActiveX‑элемент TextBox
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Установите свойство ShowDropButtonTypeWhen
            textBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus;

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


