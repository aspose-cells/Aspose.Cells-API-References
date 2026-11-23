---
title: "CheckBoxActiveXControl.IsTripleState"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CheckBoxActiveXControl. Indique comment le contrôle spécifié affichera les valeurs Null"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/istriplestate/
---
## CheckBoxActiveXControl.IsTripleState property

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
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle CheckBox ActiveX avec tous les paramètres requis
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Configurer les propriétés de base
            checkBox.Caption = "Triple State Demo";
            
            // Démontrer la propriété IsTripleState
            checkBox.IsTripleState = true; // Enable three states: Checked, Unchecked, and Indeterminate
            checkBox.Value = CheckValueType.Mixed; // Set to indeterminate state

            // Enregistrez le classeur
            workbook.Save("CheckBoxTripleStateDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


