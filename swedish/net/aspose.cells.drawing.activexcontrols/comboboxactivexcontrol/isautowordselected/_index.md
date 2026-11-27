---
title: "ComboBoxActiveXControl.IsAutoWordSelected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Anger den grundläggande enheten som används för att utöka en markering. True anger att den grundläggande enheten är ett enskilt tecken. false anger att den grundläggande enheten är ett helt ord"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isautowordselected/
---
## ComboBoxActiveXControl.IsAutoWordSelected property

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
    public class ComboBoxActiveXControlPropertyIsAutoWordSelectedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX control med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 100, 20, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera grundläggande egenskaper
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.Value = "Sample Text";

            // Demonstrera IsAutoWordSelected-egenskapen
            comboBox.IsAutoWordSelected = false;
            Console.WriteLine("IsAutoWordSelected set to: " + comboBox.IsAutoWordSelected);

            // Spara arbetsboken
            workbook.Save("ComboBoxIsAutoWordSelectedDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


