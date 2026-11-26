---
title: "LabelActiveXControl.SpecialEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LabelActiveXControl. Obtiene y establece el efecto especial del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/specialeffect/
---
## LabelActiveXControl.SpecialEffect property

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
    public class LabelActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX Label con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 100, 50,  // upperLeftRow, upperLeftColumn, height, width
                100, 50);       // heightInPx, widthInPx
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Establecer propiedades básicas
            labelControl.Caption = "Sample Label";
            labelControl.IsWordWrapped = true;

            // Demostrar la propiedad SpecialEffect
            labelControl.SpecialEffect = ControlSpecialEffectType.Raised;
            Console.WriteLine("SpecialEffect set to: " + labelControl.SpecialEffect);

            // Cambiar SpecialEffect y mostrar la diferencia
            labelControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            Console.WriteLine("SpecialEffect changed to: " + labelControl.SpecialEffect);

            // Guarda el libro de trabajo
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


