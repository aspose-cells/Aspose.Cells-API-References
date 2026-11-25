---
title: "ComboBox.SelectedIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBox. Ottiene o imposta il numero di indice dell'elemento attualmente selezionato in una casella di riepilogo o casella combinata. Basato su zero"
type: docs
url: /it/net/aspose.cells.drawing/combobox/selectedindex/
---
## ComboBox.SelectedIndex property

Ottiene o imposta il numero di indice dell'elemento attualmente selezionato in una casella di riepilogo o in una casella combinata. Basato su zero.

```csharp
public int SelectedIndex { get; set; }
```

### Osservazioni

-1 presents no item is selected.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la casella combinata
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Aggiungi una casella combinata al foglio di lavoro
            Shape shape = worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 20);
            ComboBox comboBox = (ComboBox)shape;

            // Imposta l'intervallo di input per la casella combinata
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Imposta e visualizza l'indice selezionato
            comboBox.SelectedIndex = 2; // Selects "Item 3" (zero-based index)
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);

            // Modifica l'indice selezionato e visualizza nuovamente
            comboBox.SelectedIndex = 4; // Selects "Item 5"
            Console.WriteLine("\nAfter changing selection:");
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);
        }
    }
}
```

### Vedi anche

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


