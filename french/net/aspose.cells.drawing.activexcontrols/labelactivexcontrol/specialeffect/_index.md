---
title: "LabelActiveXControl.SpecialEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "LabelActiveXControl propriété. Obtient et définit l'effet spécial du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/specialeffect/
---
## LabelActiveXControl.SpecialEffect property

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
    public class LabelActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX Label avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 100, 50,  // upperLeftRow, upperLeftColumn, height, width
                100, 50);       // heightInPx, widthInPx
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Définir les propriétés de base
            labelControl.Caption = "Sample Label";
            labelControl.IsWordWrapped = true;

            // Démontrer la propriété SpecialEffect
            labelControl.SpecialEffect = ControlSpecialEffectType.Raised;
            Console.WriteLine("SpecialEffect set to: " + labelControl.SpecialEffect);

            // Modifier SpecialEffect et montrer la différence
            labelControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            Console.WriteLine("SpecialEffect changed to: " + labelControl.SpecialEffect);

            // Enregistrez le classeur
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


