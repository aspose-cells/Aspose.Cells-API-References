---
title: "TextBoxActiveXControl.SpecialEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxActiveXControl. Obtient et définit l'effet spécial du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/specialeffect/
---
## TextBoxActiveXControl.SpecialEffect property

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
    public class TextBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX TextBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 100, 100, 0, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Définir la propriété SpecialEffect
            textBox.SpecialEffect = ControlSpecialEffectType.Bump;

            // Enregistrez le classeur
            workbook.Save("TextBoxActiveXControlSpecialEffectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


