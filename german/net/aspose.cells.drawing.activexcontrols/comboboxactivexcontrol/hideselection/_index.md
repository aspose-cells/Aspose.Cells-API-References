---
title: "ComboBoxActiveXControl.HideSelection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl property. Gibt an, ob ausgewählter Text im Steuerelement hervorgehoben angezeigt wird, wenn das Steuerelement keinen Fokus hat."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/hideselection/
---
## ComboBoxActiveXControl.HideSelection property

Gibt an, ob ausgewählter Text im Steuerelement hervorgehoben angezeigt wird, wenn das Steuerelement keinen Fokus hat.

```csharp
public bool HideSelection { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein ComboBox ActiveX-Steuerelement mit allen erforderlichen Parametern hinzu
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                10, 10, 150, 30, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Grundlegende Eigenschaften konfigurieren
            comboBox.ListRows = 5;
            comboBox.Value = "Select an item";
            
            // Füge Beispiel-Elemente unter Verwendung des korrekten Eigenschaftsnamens hinzu
            comboBox.ListFillRange = "A1:A3"; // Alternative way to set items
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // HideSelection-Eigenschaft demonstrieren
            comboBox.HideSelection = true; // Text won't show selection highlight when control loses focus

            // Speichere die Arbeitsmappe
            workbook.Save("ComboBoxHideSelectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


