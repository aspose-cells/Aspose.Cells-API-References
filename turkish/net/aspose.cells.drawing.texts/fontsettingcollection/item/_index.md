---
title: "FontSettingCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection özelliği. FontSetting'i indeks ile alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/item/
---
## FontSettingCollection indexer

İndeks ile [`FontSetting`](../../../aspose.cells/fontsetting/) alır.

```csharp
public FontSetting this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Örnekler

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

            // Belirli karakterler için yazı tipi özelliklerini ayarlayın
            Aspose.Cells.Font fo = tb.Characters(3, 5).Font;
            fo.IsSuperscript = true;
            fo.Color = Color.Red;

            // TextBody.Item özelliği aracılığıyla yazı tipine erişin
            Aspose.Cells.Font fo1 = tb.TextBody[3].Font;
            Console.WriteLine("IsSuperscript: " + fo1.IsSuperscript);
            Console.WriteLine("Color: " + fo1.Color);

            w.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


