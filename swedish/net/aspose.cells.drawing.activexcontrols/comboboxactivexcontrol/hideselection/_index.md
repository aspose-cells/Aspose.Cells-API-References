---
title: "ComboBoxActiveXControl.HideSelection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl property. Anger om markerad text i kontrollen visas som markerad när kontrollen inte har fokus"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/hideselection/
---
## ComboBoxActiveXControl.HideSelection property

Indikerar om markerad text i kontrollen visas markerad när kontrollen inte har fokus.

```csharp
public bool HideSelection { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX control med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                10, 10, 150, 30, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera grundläggande egenskaper
            comboBox.ListRows = 5;
            comboBox.Value = "Select an item";
            
            // Lägg till exempelobjekt med korrekt egenskapsnamn
            comboBox.ListFillRange = "A1:A3"; // Alternative way to set items
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Demonstrera HideSelection property
            comboBox.HideSelection = true; // Text won't show selection highlight when control loses focus

            // Spara arbetsboken
            workbook.Save("ComboBoxHideSelectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


