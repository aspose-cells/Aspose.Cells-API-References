---
title: "ListBox.SelectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBox-Eigenschaft. Gibt den Auswahlmodus der angegebenen ListBox zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/listbox/selectiontype/
---
## ListBox.SelectionType property

Ermittelt oder legt den Auswahlmodus des angegebenen Listenfelds fest.

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
    public class ListBoxPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Beispieldaten für die ListBox hinzufügen
            sheet.Cells["A1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Finance");
            sheet.Cells["A3"].PutValue("MIS");
            sheet.Cells["A4"].PutValue("R&D");

            // Füge eine ListBox hinzu
            ListBox listBox = sheet.Shapes.AddListBox(1, 0, 2, 0, 100, 80);
            
            // ListBox-Eigenschaften festlegen
            listBox.InputRange = "A1:A4";
            listBox.LinkedCell = "B1";
            
            // Demonstriere die SelectionType-Eigenschaft
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.SelectedIndex = 1; // Select "Finance"

            // Speichere die Arbeitsmappe
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


