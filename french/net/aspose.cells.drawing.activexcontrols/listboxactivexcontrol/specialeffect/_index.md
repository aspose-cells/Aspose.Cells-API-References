---
title: "ListBoxActiveXControl.SpecialEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListBoxActiveXControl. Obtient et définit l'effet spécial du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/specialeffect/
---
## ListBoxActiveXControl.SpecialEffect property

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
    public class ListBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 100, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Définir la propriété SpecialEffect
            listBox.SpecialEffect = ControlSpecialEffectType.Sunken;

            // Vérifier et afficher la valeur de SpecialEffect
            Console.WriteLine("ListBox SpecialEffect: " + listBox.SpecialEffect);

            // Enregistrez le classeur
            workbook.Save("ListBoxSpecialEffectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


