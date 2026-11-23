---
title: "RadioButtonActiveXControl.GroupName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RadioButtonActiveXControl. Obtient et définit le nom du groupe"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/groupname/
---
## RadioButtonActiveXControl.GroupName property

Obtient et définit le nom du groupe.

```csharp
public string GroupName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter deux contrôles RadioButton ActiveX
            var shape1 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 30);
            var radio1 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape1.ActiveXControl;
            
            var shape2 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 50, 100, 30);
            var radio2 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape2.ActiveXControl;

            // Définir le même nom de groupe pour les rendre mutuellement exclusifs
            radio1.GroupName = "RadioGroup1";
            radio2.GroupName = "RadioGroup1";

            // Définir les légendes
            radio1.Caption = "Option 1";
            radio2.Caption = "Option 2";

            // Enregistrez le classeur
            workbook.Save("RadioButtonGroupDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


