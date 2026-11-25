---
title: "ListBox.SelectedIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBox. Ottiene o imposta il numero di indice dell'elemento attualmente selezionato in una list box o combo box. Basato su zero"
type: docs
url: /it/net/aspose.cells.drawing/listbox/selectedindex/
---
## ListBox.SelectedIndex property

Ottiene o imposta il numero di indice dell'elemento attualmente selezionato in una casella di riepilogo o in una casella combinata. Basato su zero.

```csharp
public int SelectedIndex { get; set; }
```

### Osservazioni

-1 presents no item is selected.

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Item 0");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            
            ListBox listBox = worksheet.Shapes.AddListBox(5, 5, 100, 100, 200, 300);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            listBox.SelectedIndex = 2;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


