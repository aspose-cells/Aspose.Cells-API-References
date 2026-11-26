---
title: "ActiveXControlBase.Height"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Obtiene y establece la altura del control en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/height/
---
## ActiveXControlBase.Height property

Obtiene y establece la altura del control en unidades de puntos.

```csharp
public virtual double Height { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyHeightDemo
    {
        public static void Run()
        {
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar un RadioButton ActiveXControl
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 50);
            RadioButtonActiveXControl activeXControl = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Establecer propiedades básicas
            activeXControl.Caption = "Height Demo";
            activeXControl.IsAutoSize = false; // Disable auto-size to demonstrate Height property

            // Demostrar la propiedad Height
            Console.WriteLine("Original Height: " + activeXControl.Height);
            activeXControl.Height = 75;
            Console.WriteLine("Modified Height: " + activeXControl.Height);

            // Guarda el libro de trabajo
            workbook.Save("ActiveXControlHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


