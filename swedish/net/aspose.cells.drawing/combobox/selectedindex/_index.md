---
title: "ComboBox.SelectedIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBox‑egenskap. Hämtar eller anger indexnumret för det för närvarande valda objektet i en listbox eller kombinationsruta. Nollbaserat"
type: docs
url: /sv/net/aspose.cells.drawing/combobox/selectedindex/
---
## ComboBox.SelectedIndex property

Hämtar eller anger indexnumret för det för närvarande markerade objektet i en listbox eller kombinationsruta. Nollbaserat.

```csharp
public int SelectedIndex { get; set; }
```

### Anmärkningar

-1 presents no item is selected.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för kombinationsrutan
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Lägg till en kombinationsruta i kalkylbladet
            Shape shape = worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 20);
            ComboBox comboBox = (ComboBox)shape;

            // Ange inmatningsområdet för kombinationsrutan
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Ange och visa det valda indexet
            comboBox.SelectedIndex = 2; // Selects "Item 3" (zero-based index)
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);

            // Ändra det valda indexet och visa igen
            comboBox.SelectedIndex = 4; // Selects "Item 5"
            Console.WriteLine("\nAfter changing selection:");
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);
        }
    }
}
```

### Se även

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


