---
title: "Sınıf HorizontalPageBreak"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HorizontalPageBreak sınıfı. Yatay sayfa kesmesini temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells/horizontalpagebreak/
---
## HorizontalPageBreak class

Yatay sayfa sonunu temsil eden nesneyi kapsüller.

```csharp
public class HorizontalPageBreak
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [EndColumn](../../aspose.cells/horizontalpagebreak/endcolumn/) { get; } | Bu yatay sayfa kesmesinin son sütun indeksini alır. |
| [Row](../../aspose.cells/horizontalpagebreak/row/) { get; } | Sıfır tabanlı satır indeksini alır. |
| [StartColumn](../../aspose.cells/horizontalpagebreak/startcolumn/) { get; } | Bu yatay sayfa kesmesinin başlangıç sütun indeksini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakDemo
    {
        public static void HorizontalPageBreakExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            
            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Y30 hücresine bir sayfa kesmesi ekleyin
            int index = worksheet.HorizontalPageBreaks.Add("Y30");
            
            // Yeni eklenen yatay sayfa kesmesini alın
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
            
            // Yatay sayfa kesmesinin özelliklerini gösterin
            Console.WriteLine("Horizontal Page Break Details:");
            Console.WriteLine($"Row: {hPageBreak.Row}");
            Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
            Console.WriteLine($"End Column: {hPageBreak.EndColumn}");
            
            // Çalışma kitabını kaydedin
            workbook.Save("HorizontalPageBreakExample.xlsx");
            workbook.Save("HorizontalPageBreakExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


