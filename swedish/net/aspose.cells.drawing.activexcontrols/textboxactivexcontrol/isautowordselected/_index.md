---
title: "TextBoxActiveXControl.IsAutoWordSelected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl-egenskap. Anger den grundläggande enheten som används för att utöka en markering. True betyder att den grundläggande enheten är ett enskilt tecken. false betyder att den grundläggande enheten är ett helt ord"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautowordselected/
---
## TextBoxActiveXControl.IsAutoWordSelected property

Anger den grundläggande enheten som används för att utöka en markering. True anger att den grundläggande enheten är ett enskilt tecken. false anger att den grundläggande enheten är ett helt ord.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### Exempel

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

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


