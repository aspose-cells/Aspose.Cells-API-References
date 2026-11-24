---
title: "FontSettingCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSettingCollection-Eigenschaft. Gibt das FontSetting nach dem Index zurück."
type: docs
url: /de/net/aspose.cells.drawing.texts/fontsettingcollection/item/
---
## FontSettingCollection indexer

Ruft das [`FontSetting`](../../../aspose.cells/fontsetting/) nach dem Index ab.

```csharp
public FontSetting this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

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

            // Legen Sie Schriftarteigenschaften für bestimmte Zeichen fest.
            Aspose.Cells.Font fo = tb.Characters(3, 5).Font;
            fo.IsSuperscript = true;
            fo.Color = Color.Red;

            // Zugriff auf die Schriftart über die TextBody.Item-Eigenschaft.
            Aspose.Cells.Font fo1 = tb.TextBody[3].Font;
            Console.WriteLine("IsSuperscript: " + fo1.IsSuperscript);
            Console.WriteLine("Color: " + fo1.Color);

            w.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


