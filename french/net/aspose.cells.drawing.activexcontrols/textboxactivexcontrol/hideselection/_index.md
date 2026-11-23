---
title: "TextBoxActiveXControl.HideSelection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxActiveXControl. Indique si le texte sélectionné dans le contrôle apparaît en surbrillance lorsque le contrôle n'a pas le focus"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/hideselection/
---
## TextBoxActiveXControl.HideSelection property

Indique si le texte sélectionné dans le contrôle apparaît en surbrillance lorsque le contrôle n'a pas le focus.

```csharp
public bool HideSelection { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX TextBox à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Démontrer la propriété HideSelection
            Console.WriteLine("Initial HideSelection value: " + textBox.HideSelection);
            
            // Définir HideSelection sur true si elle est false
            if (!textBox.HideSelection)
            {
                textBox.HideSelection = true;
                Console.WriteLine("HideSelection set to: " + textBox.HideSelection);
            }

            // Enregistrez le classeur
            workbook.Save("TextBoxActiveXControlHideSelectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


