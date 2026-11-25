---
title: "ToggleButtonActiveXControl.SpecialEffect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ToggleButtonActiveXControl. Ottiene e imposta l'effetto speciale del controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/specialeffect/
---
## ToggleButtonActiveXControl.SpecialEffect property

Ottiene e imposta l'effetto speciale del controllo.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ToggleButton
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl control = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà SpecialEffect
            control.SpecialEffect = ControlSpecialEffectType.Bump;

            // Salva la cartella di lavoro
            workbook.Save("ToggleButtonSpecialEffectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


