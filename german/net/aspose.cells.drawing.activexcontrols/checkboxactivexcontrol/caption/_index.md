---
title: "CheckBoxActiveXControl.Caption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBoxActiveXControl-Eigenschaft. Ruft den beschreibenden Text ab, der auf einem Steuerelement angezeigt wird, und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/caption/
---
## CheckBoxActiveXControl.Caption property

Liest und setzt den beschreibenden Text, der auf einem Steuerelement angezeigt wird.

```csharp
public string Caption { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            // Initialisieren Sie ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein CheckBox‑ActiveX‑Steuerelement hinzufügen
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Setzen und demonstrieren Sie die Caption-Eigenschaft
            checkBoxControl.Caption = "Sample CheckBox Caption";
            checkBoxControl.Value = CheckValueType.Checked;  // Fixed: Using correct enum value

            // Speichere die Arbeitsmappe
            workbook.Save("CheckBoxCaptionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


