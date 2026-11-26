---
title: "TextBoxActiveXControl.BorderOleColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Получает и задает OLE‑цвет фона"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderolecolor/
---
## TextBoxActiveXControl.BorderOleColor property

Получает и задает ole‑цвет фона.

```csharp
public int BorderOleColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ActiveX TextBox и получите его свойство ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 100, 100, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Установите свойство BorderOleColor (стандартная система цветов Excel 12 или зелёный)
            textBox.BorderOleColor = unchecked((int)0x80000012);

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlBorderOleColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


