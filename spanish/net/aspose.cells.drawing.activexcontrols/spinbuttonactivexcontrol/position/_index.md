---
title: "SpinButtonActiveXControl.Position"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de SpinButtonActiveXControl. Obtiene y establece el valor"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/
---
## SpinButtonActiveXControl.Position property

Obtiene y establece el valor.

```csharp
public int Position { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyPositionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX SpinButton
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton,
                1, 0, 1, 0, 100, 30);

            // Obtener el control ActiveX y establecer la propiedad Position
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Position = 30;

            // Guarda el libro de trabajo
            workbook.Save("SpinButtonPositionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


