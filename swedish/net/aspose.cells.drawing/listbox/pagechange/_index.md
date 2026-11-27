---
title: "ListBox.PageChange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBox-egenskap. Anger hur mycket kontrollens värde ändras när användaren klickar på rullningslistans sida upp eller sida ner-område"
type: docs
url: /sv/net/aspose.cells.drawing/listbox/pagechange/
---
## ListBox.PageChange property

Anger hur mycket kontrollens värde ändras när användaren klickar på rullningslistans sida‑upp‑ eller sida‑ned‑område.

```csharp
public int PageChange { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ListBox-form
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 100);

            // Ställ in några poster för ListBoxen
            listBox.SetInputRange("A1:A5", false, false);
            
            // Ställ in PageChange-egenskapen
            listBox.PageChange = 2;

            // Spara arbetsboken
            workbook.Save("ListBoxPageChangeDemo.xlsx");

            // Visa PageChange-värdet
            Console.WriteLine("ListBox PageChange value: " + listBox.PageChange);
        }
    }
}
```

### Se även

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


