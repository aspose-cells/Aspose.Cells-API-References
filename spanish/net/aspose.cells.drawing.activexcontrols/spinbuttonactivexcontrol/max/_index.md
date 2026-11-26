---
title: "SpinButtonActiveXControl.Max"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SpinButtonActiveXControl. Obtiene y establece el valor máximo aceptable"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/
---
## SpinButtonActiveXControl.Max property

Obtiene y establece el valor máximo aceptable.

```csharp
public int Max { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMaxDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un control SpinButton ActiveX a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 1, 1, 1, 100, 30);
            
            // Obtén el control ActiveX y establece su propiedad Max
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Max = 100;
            
            // Guarda el libro de trabajo
            workbook.Save("SpinButtonMaxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


