---
title: "ComboBox.SelectedIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBox Eigenschaft. Liest oder setzt die Indexnummer des aktuell ausgewählten Elements in einer Listbox oder ComboBox. Nullbasiert"
type: docs
url: /de/net/aspose.cells.drawing/combobox/selectedindex/
---
## ComboBox.SelectedIndex property

Ermittelt oder legt die Indexnummer des aktuell ausgewählten Elements in einem Listenfeld oder Kombinationsfeld fest. Nullbasiert.

```csharp
public int SelectedIndex { get; set; }
```

### Hinweise

-1 presents no item is selected.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die ComboBox hinzufügen
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Eine ComboBox zum Arbeitsblatt hinzufügen
            Shape shape = worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 20);
            ComboBox comboBox = (ComboBox)shape;

            // Legen Sie den Eingabebereich für das Kombinationsfeld fest
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Ausgewählten Index festlegen und anzeigen
            comboBox.SelectedIndex = 2; // Selects "Item 3" (zero-based index)
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);

            // Ausgewählten Index ändern und erneut anzeigen
            comboBox.SelectedIndex = 4; // Selects "Item 5"
            Console.WriteLine("\nAfter changing selection:");
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);
        }
    }
}
```

### Siehe auch

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


