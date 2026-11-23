---
title: "TextBoxActiveXControl.IsWordWrapped"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxActiveXControl. Indique si le contenu du contrôle s'enroule automatiquement à la fin d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iswordwrapped/
---
## TextBoxActiveXControl.IsWordWrapped property

Indique si le contenu du contrôle passe automatiquement à la ligne à la fin d'une ligne.

```csharp
public bool IsWordWrapped { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX TextBox avec tous les paramètres requis
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox,
                1, 1, 200, 100, 0, 0);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Définir un texte qui bénéficierait du retour à la ligne
            textBox.Text = "This is a long text that should demonstrate word wrapping functionality in the TextBox ActiveX control.";

            // Vérifier et définir la propriété IsWordWrapped
            if (!textBox.IsWordWrapped)
            {
                textBox.IsWordWrapped = true;
                Console.WriteLine("Word wrapping has been enabled for the TextBox.");
            }

            // Enregistrez le classeur
            workbook.Save("TextBoxWordWrapDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


