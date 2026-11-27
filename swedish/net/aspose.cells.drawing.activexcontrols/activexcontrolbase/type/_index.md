---
title: "ActiveXControlBase.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Hämtar typen av ActiveX-kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/type/
---
## ActiveXControlBase.Type property

Hämtar typen av ActiveX-kontrollen.

```csharp
public abstract ControlType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en Label ActiveX-kontroll med korrekta parametrar
            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 100, 50, 0);
            LabelActiveXControl labelControl = (LabelActiveXControl)labelShape.ActiveXControl;
            labelControl.Caption = "Label_ActiveX";

            // Demonstrera användning av Type-egenskapen
            if (labelShape.ActiveXControl.Type == ControlType.Label)
            {
                Console.WriteLine("The control is a Label type");
                labelControl.Caption = labelControl.Caption.Replace("Label_", "MyChangedLabel_");
            }

            // Spara och verifiera
            workbook.Save("output.xlsx");
            Console.WriteLine("Label caption changed to: " + labelControl.Caption);
        }
    }
}
```

### Se även

* enum [ControlType](../../controltype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


