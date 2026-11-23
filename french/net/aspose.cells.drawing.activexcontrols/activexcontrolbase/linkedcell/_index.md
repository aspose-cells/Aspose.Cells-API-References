---
title: "ActiveXControlBase.LinkedCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ActiveXControlBase. Obtient et définit la cellule liée"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/
---
## ActiveXControlBase.LinkedCell property

Obtient et définit la cellule liée.

```csharp
public string LinkedCell { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Initialiser un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter un SpinButtonActiveXControl à la première feuille de calcul
            Aspose.Cells.Drawing.Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 
                10, 10, 100, 30, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;

            // Configurer les propriétés du bouton de défilement
            spinButton.Min = 0;
            spinButton.Max = 100;
            spinButton.Position = 50;
            spinButton.SmallChange = 1;

            // Lier le contrôle à la cellule A1
            spinButton.LinkedCell = "A1";

            // Définir la valeur de la cellule A1 pour correspondre à la position initiale
            workbook.Worksheets[0].Cells["A1"].PutValue(spinButton.Position);

            // Enregistrez le classeur
            workbook.Save("LinkedCellDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


