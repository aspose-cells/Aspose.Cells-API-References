---
title: "ToggleButtonActiveXControl.Accelerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ToggleButtonActiveXControl. Obtient et définit la touche d'accélérateur pour le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator/
---
## ToggleButtonActiveXControl.Accelerator property

Obtient et définit la touche d'accélérateur pour le contrôle.

```csharp
public char Accelerator { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ToggleButton avec les paramètres appropriés
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Définir la propriété Accelerator
            toggleButton.Accelerator = 'A';
            Console.WriteLine("ToggleButton Accelerator set to: " + toggleButton.Accelerator);

            // Effacer la propriété Accelerator
            toggleButton.Accelerator = '\0';
            Console.WriteLine("ToggleButton Accelerator cleared: " + (toggleButton.Accelerator == '\0' ? "True" : "False"));
        }
    }
}
```

### Voir aussi

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


