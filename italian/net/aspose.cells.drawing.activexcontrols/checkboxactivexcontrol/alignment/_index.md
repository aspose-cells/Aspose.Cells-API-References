---
title: "CheckBoxActiveXControl.Alignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CheckBoxActiveXControl. Ottiene e imposta la posizione della didascalia rispetto al controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/alignment/
---
## CheckBoxActiveXControl.Alignment property

Ottiene e imposta la posizione della didascalia rispetto al controllo.

```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```

### Esempi

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

### Vedi anche

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


