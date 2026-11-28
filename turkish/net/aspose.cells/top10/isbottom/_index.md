---
title: "Top10.IsBottom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Top10 özelliği. Bir üst/alt n kuralının alt n kuralı olup olmadığını alır veya ayarlar. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/top10/isbottom/
---
## Top10.IsBottom property

\"top/bottom n\" kuralının \"bottom n\" kuralı olup olmadığını alın veya ayarlayın. Varsayılan değer false.

```csharp
public bool IsBottom { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Koşullu biçimlendirme ekle
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 0 });

            // Top10 koşulu ekleyin
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Top10 özelliklerini yapılandırın
            Top10 top10 = fc.Top10;
            top10.IsBottom = true; // Highlight bottom values
            top10.IsPercent = false;
            top10.Rank = 3; // Highlight bottom 3 values

            workbook.Save("Top10IsBottomExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


