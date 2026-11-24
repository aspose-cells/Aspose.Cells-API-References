---
title: "ListBoxActiveXControl.ColumnCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBoxActiveXControl-Eigenschaft. Gibt die Anzahl der Spalten an, die in einem ComboBox oder ListBox angezeigt werden sollen."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/columncount/
---
## ListBoxActiveXControl.ColumnCount property

Beschreibt die Anzahl der Spalten, die in einem ComboBox- oder ListBox-Steuerelement angezeigt werden.

```csharp
public int ColumnCount { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyColumnCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ListBox‑ActiveX‑Steuerelement hinzu
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 1, 1, 1, 200, 100);
            var listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Setze Eigenschaften einschließlich ColumnCount.
            listBox.ColumnCount = 3;
            listBox.ListFillRange = "A1:C3"; // Sample data range for 3 columns

            // Überprüfe und gib die ColumnCount aus.
            Console.WriteLine("ListBox ColumnCount: " + listBox.ColumnCount);

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


