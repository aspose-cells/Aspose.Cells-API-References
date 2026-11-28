---
title: "Top10.Rank"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Top10 özelliği. Üst/alt n koşullu biçimlendirme kuralındaki n değerini al veya ayarla. IsPercent doğru ise değer 0 ile 100 arasında olmalıdır. Aksi takdirde 0 ile 1000 arasında olmalıdır. Varsayılan değer 10'dur."
type: docs
url: /tr/net/aspose.cells/top10/rank/
---
## Top10.Rank property

\"top/bottom n\" koşullu biçimlendirme kuralında \"n\" değerini alın veya ayarlayın. IsPercent true ise değer 0 ile 100 arasında olmalıdır. Aksi takdirde 0 ile 1000 arasında olmalıdır. Varsayılan değer 10.

```csharp
public int Rank { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyRankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            Top10 top10 = fc.Top10;
            top10.Rank = 5;

            workbook.Save("Top10RankExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


