---
title: "ListBox.SelectedItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBox-metod. Anger om objektet är markerat"
type: docs
url: /sv/net/aspose.cells.drawing/listbox/selecteditem/
---
## ListBox.SelectedItem method

Anger om objektet är markerat

```csharp
public void SelectedItem(int itemIndex, bool isSelected)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| itemIndex | Int32 | Objektets index |
| isSelected | Boolean | Om objektet är markerat. Sant betyder att detta objekt ska vara markerat. Falskt betyder att detta objekt ska vara avmarkerat. |

### Exempel

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

            // Fyll i listobjekt
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i, 0].Value = $"Item {i + 1}";
            }

            // Skapa listbox
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 150, 100) as ListBox;
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            try
            {
                // Markera och avmarkera objekt
                listBox.SelectedItem(2, true);  // Select third item (index 2)
                listBox.SelectedItem(0, true);   // Select first item (index 0)
                listBox.SelectedItem(2, false); // Deselect third item

                // Verifiera markeringar
                Console.WriteLine($"Item 0 selected: {listBox.IsSelected(0)}");
                Console.WriteLine($"Item 2 selected: {listBox.IsSelected(2)}");

                // Visa markerade celler
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

### Se även

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


