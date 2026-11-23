---
title: "ActiveXControlBase.Shadow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ActiveXControlBase. Indique s'il faut afficher une ombre"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/
---
## ActiveXControlBase.Shadow property

Indique s'il faut afficher une ombre.

```csharp
public virtual bool Shadow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            commandButton.Caption = "Shadow Button";
            commandButton.Shadow = true;

            workbook.Save("ActiveXControlShadowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


