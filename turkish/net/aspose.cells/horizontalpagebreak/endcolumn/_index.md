---
title: "HorizontalPageBreak.EndColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HorizontalPageBreak özelliği. Bu yatay sayfa kesiminin bitiş sütun indeksini alır"
type: docs
url: /tr/net/aspose.cells/horizontalpagebreak/endcolumn/
---
## HorizontalPageBreak.EndColumn property

Bu yatay sayfa kesmesinin son sütun indeksini alır.

```csharp
public int EndColumn { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Satır 5'te, sütun 2'den 4'e kadar uzanan bir yatay sayfa kesimi ekleyin
            int index = worksheet.HorizontalPageBreaks.Add(5, 2, 4);
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];

            // EndColumn özelliğini gösterin
            Console.WriteLine("Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);

            // EndColumn yalnızca okunabilir olduğundan, değiştirmek için sayfa kesimini kaldırıp yeniden eklememiz gerekir
            worksheet.HorizontalPageBreaks.RemoveAt(index);
            index = worksheet.HorizontalPageBreaks.Add(5, 2, 6);
            hPageBreak = worksheet.HorizontalPageBreaks[index];
            Console.WriteLine("Modified Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);
        }
    }
}
```

### Ayrıca Bakınız

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


