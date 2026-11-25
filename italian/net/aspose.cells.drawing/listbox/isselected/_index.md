---
title: "ListBox.IsSelected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListBox. Indica se l'elemento è selezionato"
type: docs
url: /it/net/aspose.cells.drawing/listbox/isselected/
---
## ListBox.IsSelected method

Indica se l'elemento è selezionato.

```csharp
public bool IsSelected(int itemIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| itemIndex | Int32 | L'indice dell'elemento. |

### Valore di ritorno

se l'elemento è selezionato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxMethodIsSelectedWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di riepilogo al foglio di lavoro
            ListBox listBox = worksheet.Shapes.AddListBox(0, 0, 100, 100, 200, 200);

            // Imposta gli elementi dell'elenco tramite l'intervallo di celle collegato
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            listBox.LinkedCell = "A1:A3";

            // Seleziona un elemento
            listBox.SelectedIndex = 0;

            // Verifica lo stato della selezione usando IsSelected con parametro Int32
            Console.WriteLine("Item 0 selected: " + listBox.IsSelected(0));
            Console.WriteLine("Item 1 selected: " + listBox.IsSelected(1));
            Console.WriteLine("Item 2 selected: " + listBox.IsSelected(2));
        }
    }
}
```

### Vedi anche

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


