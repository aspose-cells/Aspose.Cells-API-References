---
title: "ListBox.SelectedCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBox‑Eigenschaft. Gibt die ausgewählten Zellen zurück. Gibt null zurück, wenn der Eingabebereich nicht festgelegt ist oder kein Element ausgewählt ist"
type: docs
url: /de/net/aspose.cells.drawing/listbox/selectedcells/
---
## ListBox.SelectedCells property

Ermittelt die ausgewählten Zellen. Gibt null zurück, wenn der Eingabebereich nicht festgelegt ist oder kein Element ausgewählt ist.

```csharp
public Cell[] SelectedCells { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxPropertySelectedCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fülle Beispiel‑Daten für ListBox‑Elemente
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Erstelle eine ListBox und binde sie an den Datenbereich
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(7, 0, 100, 150, 5, 1);
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            // Wähle mehrere Elemente mit nullbasierten Indizes aus
            listBox.SelectedItem(0, true);
            listBox.SelectedItem(2, true);

            // Rufe die ausgewählten Zellen ab und zeige sie an
            Cell[] selectedCells = listBox.SelectedCells;
            Console.WriteLine("Selected Cells Count: " + selectedCells.Length);
            
            // Modifiziere die ausgewählten Zellen, um den Zugriff zu demonstrieren
            foreach (Cell cell in selectedCells)
            {
                Console.WriteLine("Selected Cell Address: " + cell.Name);
                cell.PutValue("[SELECTED] " + cell.StringValue);
            }

            workbook.Save("ListBoxSelectedCellsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../../aspose.cells/cell/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


