---
title: "CheckBoxCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxCollection-egenskap. Hämtar CheckBox-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.drawing/checkboxcollection/item/
---
## CheckBoxCollection indexer

Hämtar [`CheckBox`](../../checkbox/) elementet på det angivna indexet.

```csharp
public CheckBox this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en kryssruta i kalkylbladet
            int index = worksheet.CheckBoxes.Add(10, 10, 100, 20);
            
            // Åtkomst till checkBox med Item-egenskap (indexerare)
            Aspose.Cells.Drawing.CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Name = "CheckBox1";
            
            // Åtkomst till checkBox med index (Item-egenskap)
            Aspose.Cells.Drawing.CheckBox checkBoxByName = worksheet.CheckBoxes[0];
            
            // Skriv ut checkBox-egenskaperna
            Console.WriteLine("CheckBox Name: " + checkBoxByName.Name);
            Console.WriteLine("CheckBox Text: " + checkBoxByName.Text);
            
            // Spara arbetsboken
            workbook.Save("CheckBoxExample.xlsx");
        }
    }
}
```

### Se även

* class [CheckBox](../../checkbox/)
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


