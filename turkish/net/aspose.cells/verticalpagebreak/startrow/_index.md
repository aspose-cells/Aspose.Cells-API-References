---
title: "VerticalPageBreak.StartRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VerticalPageBreak özelliği. Dikey sayfa kesmesinin başlangıç satır indeksini alır"
type: docs
url: /tr/net/aspose.cells/verticalpagebreak/startrow/
---
## VerticalPageBreak.StartRow property

Dikey sayfa sonunun başlangıç satır indeksini alır.

```csharp
public int StartRow { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyStartRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Başlangıç satırı (2) istenen dikey sayfa kesmelerini başlangıçta ekleyin
            worksheet.VerticalPageBreaks.Add(2, 0, 10);
            VerticalPageBreak vPageBreak = worksheet.VerticalPageBreaks[0];

            // StartRow özelliğini göster
            Console.WriteLine("Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // StartRow yalnızca okunabilir olduğundan, değiştirmek için kaldırıp yeniden eklememiz gerekir
            worksheet.VerticalPageBreaks.RemoveAt(0);
            worksheet.VerticalPageBreaks.Add(5, 0, 10);
            vPageBreak = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Modified Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Çalışma kitabını kaydedin
            workbook.Save("VerticalPageBreakExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


