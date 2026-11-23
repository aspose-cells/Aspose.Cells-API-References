---
title: "CheckBoxActiveXControl.IsWordWrapped"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CheckBoxActiveXControl. Indique si le contenu du contrôle passe automatiquement à la ligne à la fin d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/iswordwrapped/
---
## CheckBoxActiveXControl.IsWordWrapped property

Indique si le contenu du contrôle passe automatiquement à la ligne à la fin d'une ligne.

```csharp
public bool IsWordWrapped { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 150, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            checkBox.Caption = "This is a long caption that should word wrap when enabled";
            checkBox.IsWordWrapped = true;
            checkBox.IsAutoSize = true;

            workbook.Save("CheckBoxWordWrapDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


