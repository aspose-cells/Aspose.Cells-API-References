---
title: "Worksheet.VerticalPageBreaks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. VerticalPageBreakCollection koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/verticalpagebreaks/
---
## Worksheet.VerticalPageBreaks property

Alır [`VerticalPageBreakCollection`](../../verticalpagebreakcollection/) koleksiyonunu.

```csharp
public VerticalPageBreakCollection VerticalPageBreaks { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVerticalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Farklı tiplerde dikey sayfa sonları ekleyin
            verticalPageBreaks.Add(0, 10, 2);
            verticalPageBreaks.Add(4);
            verticalPageBreaks.Add(5, 3);
            verticalPageBreaks.Add("G5");

            // Bir sonu kaldırın
            verticalPageBreaks.RemoveAt(1);

            // Son bilgiini yazdırın
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Break {i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [VerticalPageBreakCollection](../../verticalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


