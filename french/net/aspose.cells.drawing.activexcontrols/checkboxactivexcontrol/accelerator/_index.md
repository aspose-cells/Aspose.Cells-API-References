---
title: "CheckBoxActiveXControl.Accelerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CheckBoxActiveXControl. Obtient et définit la touche d'accélérateur pour le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/accelerator/
---
## CheckBoxActiveXControl.Accelerator property

Obtient et définit la touche d'accélérateur pour le contrôle.

```csharp
public char Accelerator { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.CheckBoxActiveXControl checkBox = (Aspose.Cells.Drawing.ActiveXControls.CheckBoxActiveXControl)shape.ActiveXControl;

            checkBox.Caption = "Check with Alt+A";
            checkBox.Accelerator = 'A';
            checkBox.IsAutoSize = true;

            workbook.Save("CheckBoxAcceleratorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


