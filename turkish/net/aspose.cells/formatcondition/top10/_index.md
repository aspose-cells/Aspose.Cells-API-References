---
title: "FormatCondition.Top10"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Koşullu biçimlendirmelerin Top10 örneğini al. Varsayılan örnek kuralı, değerleri en üst 10 aralığına düşen hücreleri vurgular. Yalnızca Top10 türü için geçerlidir."
type: docs
url: /tr/net/aspose.cells/formatcondition/top10/
---
## FormatCondition.Top10 property

Koşullu biçimlendirme'nin "Top10" örneğini al. Varsayılan örneğin kuralı, değerleri en üst 10 dilimine düşen hücreleri vurgular. Yalnızca type = Top10 için geçerlidir.

```csharp
public Top10 Top10 { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTop10Demo
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
            top10.IsPercent = true;
            top10.IsBottom = true;
            top10.Rank = 10;

            workbook.Save("FormatConditionPropertyTop10Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Top10](../../top10/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


