---
title: "SpinButtonActiveXControl.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SpinButtonActiveXControl. Obtient le type du contrôle ActiveX"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type/
---
## SpinButtonActiveXControl.Type property

Obtient le type du contrôle ActiveX.

```csharp
public override ControlType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez un contrôle ActiveX SpinButton (paramètres : left, top, width, height)
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 30, 100, 30);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Vérifiez le type du contrôle en utilisant la propriété Type
            if (spinButton.Type == ControlType.SpinButton)
            {
                // Définissez certaines propriétés spécifiques à SpinButton
                spinButton.Min = 0;
                spinButton.Max = 100;
                spinButton.Position = 50;
                spinButton.SmallChange = 1;
            }
            
            // Enregistrez le classeur
            workbook.Save("SpinButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlType](../../controltype/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


