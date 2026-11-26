---
title: "SpinButtonActiveXControl.SmallChange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SpinButtonActiveXControl. Obtiene y establece la cantidad en que cambia la propiedad Position"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/
---
## SpinButtonActiveXControl.SmallChange property

Obtiene y establece la cantidad en que cambia la propiedad Position

```csharp
public int SmallChange { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertySmallChangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un control SpinButton ActiveX a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            
            // Obtén el control ActiveX y establece la propiedad SmallChange
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.SmallChange = 5;
            
            // Guarda el libro de trabajo
            workbook.Save("SpinButtonSmallChangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


