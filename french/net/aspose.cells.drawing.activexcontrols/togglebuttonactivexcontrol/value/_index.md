---
title: "ToggleButtonActiveXControl.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ToggleButtonActiveXControl. Indique si le contrôle est coché ou non"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value/
---
## ToggleButtonActiveXControl.Value property

Indique si le contrôle est coché ou non.

```csharp
public CheckValueType Value { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ToggleButton
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Définir la valeur initiale sur Non coché
            toggleButton.Value = CheckValueType.UnChecked;

            // Vérifier et basculer la valeur si elle est Non cochée
            if (toggleButton.Value == CheckValueType.UnChecked)
            {
                toggleButton.Value = CheckValueType.Checked;
            }

            // Enregistrez le classeur
            workbook.Save("ToggleButtonDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


