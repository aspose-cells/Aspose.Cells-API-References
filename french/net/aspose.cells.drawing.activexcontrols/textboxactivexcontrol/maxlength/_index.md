---
title: "TextBoxActiveXControl.MaxLength"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxActiveXControl. Obtient et définit le nombre maximal de caractères"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/maxlength/
---
## TextBoxActiveXControl.MaxLength property

Obtient et définit le nombre maximal de caractères

```csharp
public int MaxLength { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX TextBox et obtenir sa propriété ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Définir la propriété MaxLength
            if (textBox.MaxLength == 0)
            {
                textBox.MaxLength = 30;
            }

            // Enregistrez le classeur
            workbook.Save("TextBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


