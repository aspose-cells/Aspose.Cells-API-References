---
title: "HyperlinkCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HyperlinkCollection‑egenskap. Hämtar Hyperlink‑elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/hyperlinkcollection/item/
---
## HyperlinkCollection indexer

Hämtar [`Hyperlink`](../../hyperlink/)‑elementet på det angivna indexet.

```csharp
public Hyperlink this[int index] { get; }
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

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en hyperlänk till cell A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.example.com");
            
            // Kom åt den första hyperlänken med Item‑egenskapen och ange visningstext
            worksheet.Hyperlinks[0].TextToDisplay = "Click Here";
            
            // Ställ in hyperlänkstil (blå understruken text)
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.Underline = FontUnderlineType.Single;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Se även

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


