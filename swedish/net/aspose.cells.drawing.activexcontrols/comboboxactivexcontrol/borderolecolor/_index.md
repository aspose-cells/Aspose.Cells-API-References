---
title: "ComboBoxActiveXControl.BorderOleColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Hämtar och sätter OLE-färgen för bakgrunden"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderolecolor/
---
## ComboBoxActiveXControl.BorderOleColor property

Hämtar och anger ole-färgen för bakgrunden.

```csharp
public int BorderOleColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Hämta det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                1, 1, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera grundläggande egenskaper
            comboBox.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // Demonstrera BorderOleColor-egenskapen
            comboBox.BorderOleColor = ColorTranslator.ToOle(Color.Red); // Set border color to red
            
            // Ange lite exempeltext
            comboBox.Value = "Border Color Demo";

            // Spara arbetsboken
            workbook.Save("ComboBoxBorderColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


