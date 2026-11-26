---
title: "TextBoxActiveXControl.SpecialEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Obtiene y establece el efecto especial del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/specialeffect/
---
## TextBoxActiveXControl.SpecialEffect property

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
    public class TextBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 100, 100, 0, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad SpecialEffect
            textBox.SpecialEffect = ControlSpecialEffectType.Bump;

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlSpecialEffectDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


