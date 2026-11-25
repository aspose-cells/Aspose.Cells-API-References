---
title: "ListBox.PageChange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBox. Specifica la quantità di cui il valore del controllo viene modificato quando l'utente fa clic sulla zona di avanzamento o retrocessione della barra di scorrimento"
type: docs
url: /it/net/aspose.cells.drawing/listbox/pagechange/
---
## ListBox.PageChange property

Specifica la quantità di cui il valore del controllo viene modificato quando l'utente fa clic sulla zona di avanzamento o retrocessione della barra di scorrimento.

```csharp
public int PageChange { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyPageChangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma ListBox
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 100);

            // Imposta alcuni elementi per la ListBox
            listBox.SetInputRange("A1:A5", false, false);
            
            // Imposta la proprietà PageChange
            listBox.PageChange = 2;

            // Salva la cartella di lavoro
            workbook.Save("ListBoxPageChangeDemo.xlsx");

            // Visualizza il valore di PageChange
            Console.WriteLine("ListBox PageChange value: " + listBox.PageChange);
        }
    }
}
```

### Vedi anche

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


