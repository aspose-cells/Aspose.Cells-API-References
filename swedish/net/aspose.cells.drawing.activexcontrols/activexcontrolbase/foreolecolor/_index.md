---
title: "ActiveXControlBase.ForeOleColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Hämtar och anger OLE‑färgen för förgrunden"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/
---
## ActiveXControlBase.ForeOleColor property

Hämtar och anger ole-färgen för förgrunden.

```csharp
public virtual int ForeOleColor { get; set; }
```

### Anmärkningar

Gäller inte för Image‑kontrollen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyForeOleColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CheckBox ActiveX‑kontroll med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Ställ in grundläggande egenskaper
            checkBox.Caption = "Sample CheckBox";
            checkBox.IsAutoSize = true;

            // Visa ForeOleColor‑egenskapen
            checkBox.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            checkBox.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);

            // Spara arbetsboken
            workbook.Save("ActiveXControlForeOleColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


