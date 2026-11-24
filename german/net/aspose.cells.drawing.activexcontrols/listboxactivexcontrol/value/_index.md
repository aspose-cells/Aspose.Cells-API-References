---
title: "ListBoxActiveXControl.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBoxActiveXControl Eigenschaft. Ruft den Wert des Steuerelements ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/value/
---
## ListBoxActiveXControl.Value property

Liest und setzt den Wert des Steuerelements.

```csharp
public string Value { get; set; }
```

### Hinweise

Nur wirksam, wenn [`SelectionType`](../selectiontype/) SelectionType.Single ist;

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ListBox‑ActiveX‑Steuerelement hinzu
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Grundlegende Eigenschaften festlegen
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;

            // Setze Elemente über die Value‑Eigenschaft
            listBox.Value = "Red;Green;Blue;Yellow";

            // Speichere die Arbeitsmappe
            workbook.Save("ListBoxValueDemo.xlsx");

            Console.WriteLine("ListBox with items set using Value property has been created.");
        }
    }
}
```

### Siehe auch

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


