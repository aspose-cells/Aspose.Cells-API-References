---
title: "ToggleButtonActiveXControl.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ToggleButtonActiveXControl. Indica si el control está marcado o no"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value/
---
## ToggleButtonActiveXControl.Value property

Indica si el control está marcado o no.

```csharp
public CheckValueType Value { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ToggleButton
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Establecer el valor inicial a Desmarcado
            toggleButton.Value = CheckValueType.UnChecked;

            // Verificar y alternar el valor si está Desmarcado
            if (toggleButton.Value == CheckValueType.UnChecked)
            {
                toggleButton.Value = CheckValueType.Checked;
            }

            // Guarda el libro de trabajo
            workbook.Save("ToggleButtonDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


