---
title: "ListBox.PageChange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBox‑Eigenschaft. Gibt den Betrag an, um den der Wert des Steuerelements geändert wird, wenn der Benutzer im Bereich der Bildlaufleiste nach oben oder unten klickt"
type: docs
url: /de/net/aspose.cells.drawing/listbox/pagechange/
---
## ListBox.PageChange property

Gibt den Betrag an, um den der Wert des Steuerelements geändert wird, wenn der Benutzer auf den Seiten‑auf‑oder‑ab‑Bereich der Bildlaufleiste klickt.

```csharp
public int PageChange { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine ListBox‑Form hinzu
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 100);

            // Setze einige Elemente für die ListBox
            listBox.SetInputRange("A1:A5", false, false);
            
            // Setze die PageChange‑Eigenschaft
            listBox.PageChange = 2;

            // Speichere die Arbeitsmappe
            workbook.Save("ListBoxPageChangeDemo.xlsx");

            // Zeige den PageChange‑Wert an
            Console.WriteLine("ListBox PageChange value: " + listBox.PageChange);
        }
    }
}
```

### Siehe auch

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


