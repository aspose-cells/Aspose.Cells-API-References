---
title: "FontSettingCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection egenskap. Hämtar FontSetting efter indexet"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/item/
---
## FontSettingCollection indexer

Hämtar [`FontSetting`](../../../aspose.cells/fontsetting/) efter indexet.

```csharp
public FontSetting this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook w = new Workbook();
            Worksheet s = w.Worksheets[0];

            Shape tb = s.Shapes.AddTextBox(3, 0, 7, 0, 70, 300);
            tb.Text = "Sample Text";

            // Ange teckensnittsegenskaper för specifika tecken
            Aspose.Cells.Font fo = tb.Characters(3, 5).Font;
            fo.IsSuperscript = true;
            fo.Color = Color.Red;

            // Åtkomst till font via TextBody.Item egenskap
            Aspose.Cells.Font fo1 = tb.TextBody[3].Font;
            Console.WriteLine("IsSuperscript: " + fo1.IsSuperscript);
            Console.WriteLine("Color: " + fo1.Color);

            w.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


