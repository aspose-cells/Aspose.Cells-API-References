---
title: "SpinButtonActiveXControl.Position"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SpinButtonActiveXControl. Obtient et définit la valeur"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/
---
## SpinButtonActiveXControl.Position property

Obtient et définit la valeur.

```csharp
public int Position { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyPositionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX SpinButton
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton,
                1, 0, 1, 0, 100, 30);

            // Obtenir le contrôle ActiveX et définir la propriété Position
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Position = 30;

            // Enregistrez le classeur
            workbook.Save("SpinButtonPositionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


