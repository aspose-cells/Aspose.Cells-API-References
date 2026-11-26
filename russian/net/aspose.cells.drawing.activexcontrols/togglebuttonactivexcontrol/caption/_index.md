---
title: "ToggleButtonActiveXControl.Caption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ToggleButtonActiveXControl. Получает и задает описательный текст, отображаемый на элементе управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption/
---
## ToggleButtonActiveXControl.Caption property

Получает и задает описательный текст, отображаемый на элементе управления.

```csharp
public string Caption { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 2, 0, 2, 0, 100, 30);
            ToggleButtonActiveXControl toggleButtonControl = (ToggleButtonActiveXControl)shape.ActiveXControl;
            toggleButtonControl.Caption = "ExampleButton";

            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


