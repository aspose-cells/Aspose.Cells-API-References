---
title: "SpinButtonActiveXControl.SmallChange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SpinButtonActiveXControl. Obtient et définit la quantité par laquelle la propriété Position change"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/
---
## SpinButtonActiveXControl.SmallChange property

Obtient et définit la quantité par laquelle la propriété Position change

```csharp
public int SmallChange { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertySmallChangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un contrôle ActiveX SpinButton à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            
            // Obtenez le contrôle ActiveX et définissez la propriété SmallChange
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.SmallChange = 5;
            
            // Enregistrez le classeur
            workbook.Save("SpinButtonSmallChangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


