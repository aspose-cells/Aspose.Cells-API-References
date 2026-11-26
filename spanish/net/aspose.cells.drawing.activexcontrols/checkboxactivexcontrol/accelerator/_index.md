---
title: "CheckBoxActiveXControl.Accelerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CheckBoxActiveXControl. Obtiene y establece la tecla aceleradora del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/accelerator/
---
## CheckBoxActiveXControl.Accelerator property

Obtiene y establece la tecla de acceso rápido para el control.

```csharp
public char Accelerator { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.CheckBoxActiveXControl checkBox = (Aspose.Cells.Drawing.ActiveXControls.CheckBoxActiveXControl)shape.ActiveXControl;

            checkBox.Caption = "Check with Alt+A";
            checkBox.Accelerator = 'A';
            checkBox.IsAutoSize = true;

            workbook.Save("CheckBoxAcceleratorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


