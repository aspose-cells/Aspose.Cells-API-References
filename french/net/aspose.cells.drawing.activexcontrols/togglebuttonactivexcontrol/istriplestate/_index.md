---
title: "ToggleButtonActiveXControl.IsTripleState"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ToggleButtonActiveXControl. Indique comment le contrôle spécifié affichera les valeurs Null"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/istriplestate/
---
## ToggleButtonActiveXControl.IsTripleState property

Indique comment le contrôle spécifié affichera les valeurs Null.

```csharp
public bool IsTripleState { get; set; }
```

### Remarques

| **Paramètre** | **Description** |
| --- | --- |
| Vrai | Le contrôle parcourra les états pour les valeurs Oui, Non et Null. Le contrôle apparaît atténué (gris) lorsque sa propriété Value est définie sur Null. |
| Faux | (Par défaut) Le contrôle parcourra les états pour les valeurs Oui et Non. Les valeurs Null s'affichent comme si c'était des valeurs Non. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX ToggleButton
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 0, 1, 0, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Définir la propriété IsTripleState sur vrai
            toggleButton.IsTripleState = true;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Modifier la propriété IsTripleState en faux
            toggleButton.IsTripleState = false;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Enregistrez le classeur
            workbook.Save("ToggleButtonIsTripleStateDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


