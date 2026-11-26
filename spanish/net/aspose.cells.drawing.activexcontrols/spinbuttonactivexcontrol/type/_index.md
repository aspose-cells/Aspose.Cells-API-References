---
title: "SpinButtonActiveXControl.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SpinButtonActiveXControl. Obtiene el tipo del control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type/
---
## SpinButtonActiveXControl.Type property

Obtiene el tipo del control ActiveX.

```csharp
public override ControlType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agrega un control ActiveX SpinButton (parámetros: left, top, width, height)
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 30, 100, 30);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Verifica el tipo de control usando la propiedad Type
            if (spinButton.Type == ControlType.SpinButton)
            {
                // Establece algunas propiedades específicas de SpinButton
                spinButton.Min = 0;
                spinButton.Max = 100;
                spinButton.Position = 50;
                spinButton.SmallChange = 1;
            }
            
            // Guarda el libro de trabajo
            workbook.Save("SpinButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlType](../../controltype/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


