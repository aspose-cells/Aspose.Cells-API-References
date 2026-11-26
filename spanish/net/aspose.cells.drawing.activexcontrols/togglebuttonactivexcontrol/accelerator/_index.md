---
title: "ToggleButtonActiveXControl.Accelerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ToggleButtonActiveXControl. Obtiene y establece la tecla de acceso rápido para el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator/
---
## ToggleButtonActiveXControl.Accelerator property

Obtiene y establece la tecla de acceso rápido para el control.

```csharp
public char Accelerator { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ToggleButton con los parámetros adecuados
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad Accelerator
            toggleButton.Accelerator = 'A';
            Console.WriteLine("ToggleButton Accelerator set to: " + toggleButton.Accelerator);

            // Borrar la propiedad Accelerator
            toggleButton.Accelerator = '\0';
            Console.WriteLine("ToggleButton Accelerator cleared: " + (toggleButton.Accelerator == '\0' ? "True" : "False"));
        }
    }
}
```

### Ver también

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


