---
title: "TextBoxActiveXControl.IsAutoWordSelected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt die Basiseinheit an, die zum Erweitern einer Auswahl verwendet wird. True gibt an, dass die Basiseinheit ein einzelnes Zeichen ist. false gibt an, dass die Basiseinheit ein ganzes Wort ist."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautowordselected/
---
## TextBoxActiveXControl.IsAutoWordSelected property

Gibt die Basiseinheit an, die zum Erweitern einer Auswahl verwendet wird. True gibt an, dass die Basiseinheit ein einzelnes Zeichen ist. false gibt an, dass die Basiseinheit ein ganzes Wort ist.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsAutoWordSelectedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 0, 0, 1, 1, 200, 30);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)textBoxShape.ActiveXControl;

            Console.WriteLine("Initial IsAutoWordSelected: " + textBoxControl.IsAutoWordSelected);

            if (!textBoxControl.IsAutoWordSelected)
            {
                textBoxControl.IsAutoWordSelected = true;
            }

            Console.WriteLine("Final IsAutoWordSelected: " + textBoxControl.IsAutoWordSelected);
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


