---
title: "CheckBoxActiveXControl.Alignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CheckBoxActiveXControl. Obtient et définit la position de la légende par rapport au contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/alignment/
---
## CheckBoxActiveXControl.Alignment property

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
    public class CheckBoxActiveXControlPropertyAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            checkBox.Caption = "Sample CheckBox";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.Checked;

            workbook.Save("CheckBoxAlignmentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


