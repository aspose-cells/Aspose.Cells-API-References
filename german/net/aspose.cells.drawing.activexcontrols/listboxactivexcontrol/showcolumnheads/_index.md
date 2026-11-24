---
title: "ListBoxActiveXControl.ShowColumnHeads"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBoxActiveXControl-Eigenschaft. Gibt an, ob Spaltenüberschriften angezeigt werden"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/showcolumnheads/
---
## ListBoxActiveXControl.ShowColumnHeads property

Gibt an, ob Spaltenüberschriften angezeigt werden.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein ListBox ActiveX-Steuerelement mit allen erforderlichen Parametern hinzufügen
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ListBox, 
                1, 1, 100, 100,  // Left, Top, Width, Height
                0, 0);           // UpperLeftRow, UpperLeftColumn

            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Legen Sie Eigenschaften für die ListBox fest
            listBox.ColumnCount = 2;
            listBox.ListWidth = 150;
            listBox.ShowColumnHeads = true; // Demonstrate ShowColumnHeads property

            // Fügen Sie einige Beispieldaten hinzu
            listBox.Value = "Header1\tHeader2\nItem1\tData1\nItem2\tData2";

            // Speichere die Arbeitsmappe
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


