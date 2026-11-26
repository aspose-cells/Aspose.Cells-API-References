---
title: "CommandButtonActiveXControl.Caption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "CommandButtonActiveXControl property. Получает и задает описательный текст, отображаемый на элементе управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/caption/
---
## CommandButtonActiveXControl.Caption property

Получает и задает описательный текст, отображаемый на элементе управления.

```csharp
public string Caption { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl commandButton = (Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl)shape.ActiveXControl;

            // Продемонстрируйте использование свойства Caption
            commandButton.Caption = "Click Me";
            commandButton.Width = 150;
            commandButton.Height = 50;
            commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);

            workbook.Save("CommandButtonCaptionDemo.xlsx");
        }
    }
}
```

### См. также

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


