---
title: "TextBoxActiveXControl.BorderOleColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Ruft die Ole-Farbe des Hintergrunds ab und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderolecolor/
---
## TextBoxActiveXControl.BorderOleColor property

Liest und schreibt die OLE-Farbe des Hintergrunds.

```csharp
public int BorderOleColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ActiveX-TextBox-Steuerelement hinzu und rufen Sie dessen ActiveXControl-Eigenschaft ab
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 100, 100, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Setzen Sie die BorderOleColor-Eigenschaft (Excel-Standardfarbsystem 12 oder Grün)
            textBox.BorderOleColor = unchecked((int)0x80000012);

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxActiveXControlBorderOleColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


