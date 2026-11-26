---
title: "SpinButtonActiveXControl.Min"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de SpinButtonActiveXControl. Obtiene y establece el valor mínimo aceptable"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/
---
## SpinButtonActiveXControl.Min property

Obtiene y establece el valor mínimo aceptable.

```csharp
public int Min { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMinDemo
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
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Establecer la propiedad Min del SpinButton
            spinButton.Min = 0;
            
            // Establezca otras propiedades para demostrar la funcionalidad
            spinButton.Max = 100;
            spinButton.Position = 50;
            
            // Guarda el libro de trabajo
            workbook.Save("SpinButtonMinDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


