---
title: "RadioButtonActiveXControl.Alignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RadioButtonActiveXControl. Obtient et définit la position de la légende par rapport au contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/alignment/
---
## RadioButtonActiveXControl.Alignment property

Obtient et définit la position de la Caption par rapport au contrôle.

```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyAlignmentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une nouvelle collection de formes et ajouter le contrôle ActiveX
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.RadioButton, 1, 1, 100, 30, 0, 0);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;
            
            // Définir la propriété Alignment
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            
            // Enregistrez le classeur
            workbook.Save("RadioButtonAlignmentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


