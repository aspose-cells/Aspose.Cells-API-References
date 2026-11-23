---
title: "TextBoxActiveXControl.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxActiveXControl. Obtient et définit le texte du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/text/
---
## TextBoxActiveXControl.Text property

Obtient et définit le texte du contrôle.

```csharp
public string Text { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un contrôle ActiveX TextBox à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            
            // Obtenez le contrôle ActiveX et définissez son texte
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
            textBox.Text = "This is a test.";
            
            // Enregistrez le classeur
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


