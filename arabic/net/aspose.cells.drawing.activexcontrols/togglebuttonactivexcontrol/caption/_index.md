---
title: "ToggleButtonActiveXControl.Caption"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ToggleButtonActiveXControl. تحصل وتضبط النص الوصفي الذي يظهر على عنصر التحكم"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption/
---
## ToggleButtonActiveXControl.Caption property

يحصل ويضبط النص الوصفي الذي يظهر على التحكم.

```csharp
public string Caption { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


