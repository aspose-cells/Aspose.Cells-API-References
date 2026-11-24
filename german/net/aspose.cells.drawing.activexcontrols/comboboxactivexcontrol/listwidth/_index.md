---
title: "ComboBoxActiveXControl.ListWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl-Eigenschaft. Gibt die Breite in Punkten zurück und legt sie fest."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listwidth/
---
## ComboBoxActiveXControl.ListWidth property

Liest und schreibt die Breite in Punkten.

```csharp
public double ListWidth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die ComboBox hinzufügen
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");

            // Füge ein ComboBox ActiveX-Steuerelement mit allen erforderlichen Parametern hinzu
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1,  // left
                1,  // top
                100, // width
                30,  // height
                0,   // image width (unused for ComboBox)
                0    // image height (unused for ComboBox)
            );
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // ListWidth-Eigenschaft festlegen, um die Dropdown-Breite zu steuern
            comboBox.ListWidth = 150;
            comboBox.ListRows = 3;
            comboBox.LinkedCell = "A1:A3";

            // Speichere die Arbeitsmappe
            workbook.Save("ComboBoxListWidthDemo.xlsx");

            Console.WriteLine("ComboBox ListWidth set to: " + comboBox.ListWidth);
        }
    }
}
```

### Siehe auch

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


