---
title: "TextBoxActiveXControl.ShowDropButtonTypeWhen"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxActiveXControl. Spécifie le symbole affiché sur le bouton déroulant"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen/
---
## TextBoxActiveXControl.ShowDropButtonTypeWhen property

Spécifie le symbole affiché sur le bouton déroulant

```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyShowDropButtonTypeWhenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX TextBox
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Définir la propriété ShowDropButtonTypeWhen
            textBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus;

            // Enregistrez le classeur
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


