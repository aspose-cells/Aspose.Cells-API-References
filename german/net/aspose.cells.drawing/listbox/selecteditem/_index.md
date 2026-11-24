---
title: "ListBox.SelectedItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBox-Methode. Legt fest, ob das Element ausgewählt ist"
type: docs
url: /de/net/aspose.cells.drawing/listbox/selecteditem/
---
## ListBox.SelectedItem method

Legt fest, ob das Element ausgewählt ist.

```csharp
public void SelectedItem(int itemIndex, bool isSelected)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| itemIndex | Int32 | Der Elementindex |
| isSelected | Boolean | Gibt an, ob das Element ausgewählt ist. Wahr bedeutet, dass dieses Element ausgewählt sein soll. Falsch bedeutet, dass dieses Element nicht ausgewählt sein soll. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxMethodSelectedItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Listenelemente befüllen
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i, 0].Value = $"Item {i + 1}";
            }

            // ListBox erstellen
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 150, 100) as ListBox;
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            try
            {
                // Elemente auswählen und abwählen
                listBox.SelectedItem(2, true);  // Select third item (index 2)
                listBox.SelectedItem(0, true);   // Select first item (index 0)
                listBox.SelectedItem(2, false); // Deselect third item

                // Auswahlen überprüfen
                Console.WriteLine($"Item 0 selected: {listBox.IsSelected(0)}");
                Console.WriteLine($"Item 2 selected: {listBox.IsSelected(2)}");

                // Ausgewählte Zellen anzeigen
                Console.WriteLine("\nSelected Items:");
                foreach (Cell cell in listBox.SelectedCells)
                {
                    Console.WriteLine(cell.Value);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ListBoxMethodSelectedItemWithInt32BooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


