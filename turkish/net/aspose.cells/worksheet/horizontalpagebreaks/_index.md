---
title: "Worksheet.HorizontalPageBreaks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. HorizontalPageBreakCollection koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/horizontalpagebreaks/
---
## Worksheet.HorizontalPageBreaks property

[`HorizontalPageBreakCollection`](../../horizontalpagebreakcollection/) koleksiyonunu alır.

```csharp
public HorizontalPageBreakCollection HorizontalPageBreaks { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı yollarla yatay sayfa sonları ekleyin
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            worksheet.HorizontalPageBreaks.Add(15, 2);
            worksheet.HorizontalPageBreaks.Add("G5");

            // İlk sayfa sonunu kaldırın
            worksheet.HorizontalPageBreaks.RemoveAt(0);

            // Çıktıları kaydedin
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
            workbook.Save("HorizontalPageBreaksDemo.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* class [HorizontalPageBreakCollection](../../horizontalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


