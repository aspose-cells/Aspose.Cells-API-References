---
title: "ActiveXControl.IsTransparent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ActiveXControl. Indique si le contrôle est transparent"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/
---
## ActiveXControl.IsTransparent property

Indique si le contrôle est transparent.

```csharp
public bool IsTransparent { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsTransparentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour héberger le contrôle ActiveX avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 200, 50, 
                0, 0); // Adding missing parameters for upperLeftRow, upperLeftColumn, height, width, left, top

            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Définir les propriétés du contrôle
            label.Caption = "Sample Label";
            label.IsTransparent = false; // Demonstrating IsTransparent property

            // Vérifier et afficher la propriété IsTransparent
            Console.WriteLine("Label IsTransparent property: " + label.IsTransparent);

            // Modifier la transparence et vérifier à nouveau
            label.IsTransparent = true;
            Console.WriteLine("Label IsTransparent property after change: " + label.IsTransparent);

            // Enregistrez le classeur
            workbook.Save("ActiveXControlIsTransparentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


