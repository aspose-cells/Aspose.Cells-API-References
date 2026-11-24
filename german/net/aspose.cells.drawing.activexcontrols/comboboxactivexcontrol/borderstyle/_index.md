---
title: "ComboBoxActiveXControl.BorderStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl-Eigenschaft. Gibt den vom Steuerelement verwendeten Rahmentyp zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderstyle/
---
## ComboBoxActiveXControl.BorderStyle property

Liest und schreibt den Typ des vom Steuerelement verwendeten Rahmens.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Demonstrieren Sie die BorderStyle-Eigenschaft
            comboBox.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            comboBox.BorderOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);

            // Grundlegende Eigenschaften für die Funktionalität festlegen
            comboBox.ListRows = 5;
            comboBox.Value = "Sample Text";

            workbook.Save("ComboBoxBorderStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlBorderType](../../controlbordertype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


