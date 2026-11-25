---
title: "ListBox.SelectedItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListBox. Imposta se l'elemento è selezionato"
type: docs
url: /it/net/aspose.cells.drawing/listbox/selecteditem/
---
## ListBox.SelectedItem method

Imposta se l'elemento è selezionato

```csharp
public void SelectedItem(int itemIndex, bool isSelected)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| itemIndex | Int32 | L'indice dell'elemento |
| isSelected | Booleano | Indica se l'elemento è selezionato. True significa che questo elemento dovrebbe essere selezionato. False significa che questo elemento dovrebbe essere deselezionato. |

### Esempi

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

            // Popola gli elementi della lista
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i, 0].Value = $"Item {i + 1}";
            }

            // Crea una list box
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 150, 100) as ListBox;
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            try
            {
                // Seleziona e deseleziona gli elementi
                listBox.SelectedItem(2, true);  // Select third item (index 2)
                listBox.SelectedItem(0, true);   // Select first item (index 0)
                listBox.SelectedItem(2, false); // Deselect third item

                // Verifica le selezioni
                Console.WriteLine($"Item 0 selected: {listBox.IsSelected(0)}");
                Console.WriteLine($"Item 2 selected: {listBox.IsSelected(2)}");

                // Visualizza le celle selezionate
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

### Vedi anche

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


