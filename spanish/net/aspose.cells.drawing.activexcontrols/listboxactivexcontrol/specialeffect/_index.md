---
title: "ListBoxActiveXControl.SpecialEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ListBoxActiveXControl propiedad. Obtiene y establece el efecto especial del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/specialeffect/
---
## ListBoxActiveXControl.SpecialEffect property

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
    public class ListBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 100, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Establece la propiedad SpecialEffect
            listBox.SpecialEffect = ControlSpecialEffectType.Sunken;

            // Verifica y muestra el valor de SpecialEffect
            Console.WriteLine("ListBox SpecialEffect: " + listBox.SpecialEffect);

            // Guarda el libro de trabajo
            workbook.Save("ListBoxSpecialEffectDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


