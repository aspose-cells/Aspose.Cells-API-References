---
title: "ListBox.IsSelected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBox-metod. Anger om posten är markerad"
type: docs
url: /sv/net/aspose.cells.drawing/listbox/isselected/
---
## ListBox.IsSelected method

Indikerar om objektet är markerat.

```csharp
public bool IsSelected(int itemIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| itemIndex | Int32 | Postens index. |

### Returvärde

om posten är markerad.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en listbox i kalkylbladet
            ListBox listBox = worksheet.Shapes.AddListBox(0, 0, 100, 100, 200, 200);

            // Ställ in listposter via det länkade cellintervallet
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            listBox.LinkedCell = "A1:A3";

            // Välj ett objekt
            listBox.SelectedIndex = 0;

            // Kontrollera markeringsstatus med IsSelected och Int32-parameter
            Console.WriteLine("Item 0 selected: " + listBox.IsSelected(0));
            Console.WriteLine("Item 1 selected: " + listBox.IsSelected(1));
            Console.WriteLine("Item 2 selected: " + listBox.IsSelected(2));
        }
    }
}
```

### Se även

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


