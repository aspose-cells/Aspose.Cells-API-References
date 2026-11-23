---
title: "ToggleButtonActiveXControl.SpecialEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ToggleButtonActiveXControl. Obtient et définit l'effet spécial du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/specialeffect/
---
## ToggleButtonActiveXControl.SpecialEffect property

Obtient et définit l'effet spécial du contrôle.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ToggleButton
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl control = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Définir la propriété SpecialEffect
            control.SpecialEffect = ControlSpecialEffectType.Bump;

            // Enregistrez le classeur
            workbook.Save("ToggleButtonSpecialEffectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


