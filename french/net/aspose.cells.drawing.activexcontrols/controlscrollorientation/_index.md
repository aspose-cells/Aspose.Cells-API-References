---
title: "Énumération ControlScrollOrientation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.ActiveXControls.ControlScrollOrientation. Représente le type d'orientation du défilement"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/controlscrollorientation/
---
## ControlScrollOrientation enumeration

Représente le type d'orientation du défilement

```csharp
public enum ControlScrollOrientation
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Auto | `3` | Le contrôle est rendu horizontalement lorsque la largeur du contrôle est supérieure à sa hauteur. Le contrôle est rendu verticalement sinon. |
| Vertical | `0` | Le contrôle est rendu verticalement. |
| Horizontal | `1` | Le contrôle est rendu horizontalement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollOrientationDemo
    {
        public static void ControlScrollOrientationExample()
        {
            // Initialiser un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter un ScrollBarActiveXControl à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 50);
            ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Définir les propriétés du ScrollBarActiveXControl
            activeXControl.LargeChange = 5;
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            // Démontrer la définition de l'orientation en utilisant l'énumération ControlScrollOrientation
            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Enregistrez le classeur
            workbook.Save("ControlScrollOrientationExample.xlsx");
            workbook.Save("ControlScrollOrientationExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


