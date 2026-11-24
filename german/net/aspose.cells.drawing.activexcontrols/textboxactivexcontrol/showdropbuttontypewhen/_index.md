---
title: "TextBoxActiveXControl.ShowDropButtonTypeWhen"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen/
---
## TextBoxActiveXControl.ShowDropButtonTypeWhen property

Gibt das Symbol an, das auf der Dropdown-Schaltfläche angezeigt wird

```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyShowDropButtonTypeWhenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein ActiveX-TextBox-Steuerelement hinzufügen
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Setzen Sie die ShowDropButtonTypeWhen-Eigenschaft
            textBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus;

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


