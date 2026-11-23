---
title: "TextBoxActiveXControl.DropButtonStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxActiveXControl. Spécifie le symbole affiché sur le bouton déroulant"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/dropbuttonstyle/
---
## TextBoxActiveXControl.DropButtonStyle property

Spécifie le symbole affiché sur le bouton déroulant

```csharp
public DropButtonStyle DropButtonStyle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyDropButtonStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez un contrôle TextBox ActiveX
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 1, 1, 100, 50, 100, 50);
            ActiveXControl control = shape.ActiveXControl;
            
            // Convertissez en TextBoxActiveXControl pour accéder aux propriétés spécifiques de TextBox
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)control;
            
            // Définissez la propriété DropButtonStyle
            textBoxControl.DropButtonStyle = DropButtonStyle.Arrow;
            
            // Enregistrez le classeur
            workbook.Save("TextBoxActiveXControlDropButtonStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [DropButtonStyle](../../dropbuttonstyle/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


