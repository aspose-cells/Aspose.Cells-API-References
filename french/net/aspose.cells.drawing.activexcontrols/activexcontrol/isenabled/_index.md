---
title: "ActiveXControl.IsEnabled"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ActiveXControl. Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/
---
## ActiveXControl.IsEnabled property

Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur.

```csharp
public bool IsEnabled { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsEnabledDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 0, 1, 0, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
            checkBox.IsEnabled = true;
            checkBox.GroupName = "Sheet1";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.UnChecked;

            Console.WriteLine("IsEnabled state: " + checkBox.IsEnabled);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


