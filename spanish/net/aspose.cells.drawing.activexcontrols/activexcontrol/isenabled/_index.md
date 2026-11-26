---
title: "ActiveXControl.IsEnabled"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ActiveXControl. Indica si el control puede recibir el foco y responder a eventos generados por el usuario"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/
---
## ActiveXControl.IsEnabled property

Indica si el control puede recibir el foco y responder a eventos generados por el usuario.

```csharp
public bool IsEnabled { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsEnabledDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 0, 1, 0, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
            checkBox.IsEnabled = true;
            checkBox.GroupName = "Sheet1";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.UnChecked;

            Console.WriteLine("IsEnabled state: " + checkBox.IsEnabled);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


