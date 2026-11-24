---
title: "ListBoxActiveXControl.SelectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBoxActiveXControl-Eigenschaft. Gibt an, ob das Steuerelement mehrere Auswahlen zulässt."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/selectiontype/
---
## ListBoxActiveXControl.SelectionType property

Gibt an, ob das Steuerelement Mehrfachauswahl zulässt.

```csharp
public SelectionType SelectionType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // ListBox ActiveX-Steuerelement hinzufügen
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // ListBox-Eigenschaften konfigurieren
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            
            // Demonstriere die SelectionType-Eigenschaft
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.Value = "Apple;Banana;Cherry";

            // Speichere die Arbeitsmappe
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");

            Console.WriteLine("ListBox with Single SelectionType created successfully.");
        }
    }
}
```

### Siehe auch

* enum [SelectionType](../../../aspose.cells.drawing/selectiontype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


