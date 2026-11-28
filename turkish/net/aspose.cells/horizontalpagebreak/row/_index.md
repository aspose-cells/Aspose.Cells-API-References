---
title: "HorizontalPageBreak.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HorizontalPageBreak özelliği. Sıfır tabanlı satır indeksini alır"
type: docs
url: /tr/net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

Sıfır tabanlı satır indeksini alır.

```csharp
public int Row { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yatay sayfa kesimleri ekleyin
            worksheet.HorizontalPageBreaks.Add(6);
            worksheet.HorizontalPageBreaks.Add(12);

            // Yatay sayfa kesimleri koleksiyonunu alın
            HorizontalPageBreakCollection breaks = worksheet.HorizontalPageBreaks;

            // Sayfa kesimlerinin satır numaralarını gösterin
            Console.WriteLine("Page break at row: " + breaks[0].Row);
            Console.WriteLine("Page break at row: " + breaks[1].Row);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


