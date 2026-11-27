---
title: "TextBoxActiveXControl.ScrollBars"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl egenskap. Anger om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars/
---
## TextBoxActiveXControl.ScrollBars property

Anger om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en ny formsamling och lägg till ActiveX-kontroll
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
            
            // Ange ScrollBars-egenskapen till vertikal
            textBox.ScrollBars = ControlScrollBarType.BarsVertical;
            
            // Spara arbetsboken
            workbook.Save("TextBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


