---
title: "Énumération ControlScrollBarType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType enum. Représente le type de barre de défilement"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/controlscrollbartype/
---
## ControlScrollBarType enumeration

Représente le type de barre de défilement.

```csharp
public enum ControlScrollBarType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Affiche aucune barre de défilement. |
| Horizontal | `1` | Affiche une barre de défilement horizontale. |
| BarsVertical | `2` | Affiche une barre de défilement verticale. |
| BarsBoth | `3` | Affiche à la fois une barre de défilement horizontale et une verticale. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollBarTypeDemo
    {
        public static void ControlScrollBarTypeExample()
        {
            // Initialiser un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ListBox à la feuille de calcul
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            ListBoxActiveXControl listBoxControl = (ListBoxActiveXControl)shape.ActiveXControl;

            // Définissez la propriété ScrollBars pour afficher à la fois les barres de défilement horizontales et verticales
            listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;

            // Enregistrez le classeur
            workbook.Save("ControlScrollBarTypeExample.xlsx");
            workbook.Save("ControlScrollBarTypeExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


