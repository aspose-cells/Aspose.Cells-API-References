---
title: "ToggleButtonActiveXControl.SpecialEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ToggleButtonActiveXControl. Obtiene y establece el efecto especial del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/specialeffect/
---
## ToggleButtonActiveXControl.SpecialEffect property

Obtiene y establece el efecto especial del control.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ToggleButton
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl control = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad SpecialEffect
            control.SpecialEffect = ControlSpecialEffectType.Bump;

            // Guarda el libro de trabajo
            workbook.Save("ToggleButtonSpecialEffectDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


