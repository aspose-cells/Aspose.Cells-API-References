---
title: "LabelActiveXControl.BorderOleColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LabelActiveXControl. Obtient et définit la couleur OLE de l’arrière-plan"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/borderolecolor/
---
## LabelActiveXControl.BorderOleColor property

Obtient et définit la couleur ole de l'arrière-plan.

```csharp
public int BorderOleColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX Label
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Label, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl labelControl = 
                (Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl)shape.ActiveXControl;

            // Définir les propriétés
            labelControl.Caption = "Sample Label";
            labelControl.BorderOleColor = -2147483642; // Set border color (OLE_COLOR)
            labelControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // Enregistrez le classeur
            workbook.Save("LabelActiveXControlBorderOleColorDemo.xlsx");

            // Afficher la couleur de la bordure
            Console.WriteLine("BorderOleColor: " + labelControl.BorderOleColor);
        }
    }
}
```

### Voir aussi

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


