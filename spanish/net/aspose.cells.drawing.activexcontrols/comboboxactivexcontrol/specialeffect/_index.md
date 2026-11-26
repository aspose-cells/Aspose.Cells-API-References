---
title: "ComboBoxActiveXControl.SpecialEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Obtiene y establece el efecto especial del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/specialeffect/
---
## ComboBoxActiveXControl.SpecialEffect property

Obtiene y establece el efecto especial del control.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 1, 0, 1, 0, 100, 30);
            var control = (ComboBoxActiveXControl)shape.ActiveXControl;

            control.SpecialEffect = ControlSpecialEffectType.Sunken;
            control.ListRows = 8;
            control.ColumnCount = 1;

            workbook.Save("output.xls", SaveFormat.Excel97To2003);
        }
    }
}
```

### Ver también

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


