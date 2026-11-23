---
title: "TextBoxActiveXControl.EnterFieldBehavior"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxActiveXControl. Spécifie le comportement de sélection lors de l'entrée dans le contrôle. True indique que la sélection reste inchangée depuis la dernière fois que le contrôle était actif. False indique que tout le texte du contrôle sera sélectionné lors de l'entrée dans le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterfieldbehavior/
---
## TextBoxActiveXControl.EnterFieldBehavior property

Spécifie le comportement de sélection lors de l'entrée dans le contrôle. True indique que la sélection reste inchangée depuis la dernière fois que le contrôle était actif. False indique que tout le texte du contrôle sera sélectionné lors de l'entrée dans le contrôle.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyEnterFieldBehaviorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un contrôle TextBox ActiveX avec les paramètres corrects
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Démontrez la propriété EnterFieldBehavior
            Console.WriteLine("Initial EnterFieldBehavior: " + textBox.EnterFieldBehavior);
            
            // Basculez la propriété EnterFieldBehavior
            textBox.EnterFieldBehavior = !textBox.EnterFieldBehavior;
            Console.WriteLine("Toggled EnterFieldBehavior: " + textBox.EnterFieldBehavior);

            // Définissez EnterFieldBehavior sur true explicitement
            textBox.EnterFieldBehavior = true;
            Console.WriteLine("Final EnterFieldBehavior: " + textBox.EnterFieldBehavior);
        }
    }
}
```

### Voir aussi

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


