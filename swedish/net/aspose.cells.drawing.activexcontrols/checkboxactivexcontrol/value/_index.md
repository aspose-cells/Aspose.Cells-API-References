---
title: "CheckBoxActiveXControl.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl-egenskap. Anger om kontrollen är markerad eller inte"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/value/
---
## CheckBoxActiveXControl.Value property

Anger om kontrollen är markerad eller inte.

```csharp
public CheckValueType Value { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CheckBox ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Ange grundläggande egenskaper inklusive Value
            checkBox.Caption = "Check Me";
            checkBox.Value = CheckValueType.Checked; // Demonstrating Value property usage

            // Spara arbetsboken
            workbook.Save("CheckBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


