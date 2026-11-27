---
title: "ComboBoxActiveXControl.MaxLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl property. Hämtar och anger det maximala antalet tecken"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/maxlength/
---
## ComboBoxActiveXControl.MaxLength property

Hämtar och anger det maximala antalet tecken

```csharp
public int MaxLength { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                5, 0, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Ställ in MaxLength property och andra väsentliga egenskaper
            comboBox.MaxLength = 10; // Restrict input to 10 characters
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;
            comboBox.Value = "Test";

            // Spara arbetsboken
            workbook.Save("ComboBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


