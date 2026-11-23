---
title: "TextBoxActiveXControl.ScrollBars"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxActiveXControl. Indique si le contrôle possède des barres de défilement verticales, horizontales, les deux ou aucune"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars/
---
## TextBoxActiveXControl.ScrollBars property

Indique si le contrôle possède des barres de défilement verticales, des barres de défilement horizontales, les deux ou aucune.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une nouvelle collection de formes et ajouter le contrôle ActiveX
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
            
            // Définir la propriété ScrollBars sur vertical
            textBox.ScrollBars = ControlScrollBarType.BarsVertical;
            
            // Enregistrez le classeur
            workbook.Save("TextBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


