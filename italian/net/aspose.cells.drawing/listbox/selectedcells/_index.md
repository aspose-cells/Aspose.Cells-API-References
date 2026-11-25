---
title: "ListBox.SelectedCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBox. Restituisce le celle selezionate. Restituisce null se l'intervallo di input non è impostato o se nessun elemento è selezionato"
type: docs
url: /it/net/aspose.cells.drawing/listbox/selectedcells/
---
## ListBox.SelectedCells property

Restituisce le celle selezionate. Restituisce null se l'intervallo di input non è impostato o nessun elemento è selezionato

```csharp
public Cell[] SelectedCells { get; }
```

### Esempi

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

            // Popola dati di esempio per gli elementi della ListBox
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Crea una ListBox e collegala all'intervallo di dati
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(7, 0, 100, 150, 5, 1);
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            // Seleziona più elementi usando indici basati su zero
            listBox.SelectedItem(0, true);
            listBox.SelectedItem(2, true);

            // Recupera e visualizza le celle selezionate
            Cell[] selectedCells = listBox.SelectedCells;
            Console.WriteLine("Selected Cells Count: " + selectedCells.Length);
            
            // Modifica le celle selezionate per dimostrare l'accesso
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

### Vedi anche

* class [Cell](../../../aspose.cells/cell/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


