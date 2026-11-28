---
title: "Range.CopyStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range metodu. Stil ayarlarını bir kaynak aralıktan kopyalar"
type: docs
url: /tr/net/aspose.cells/range/copystyle/
---
## Range.CopyStyle method

Kaynak bir aralıktan stil ayarlarını kopyalar.

```csharp
public void CopyStyle(Range range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | Range | Kaynak [`Range`](../) nesnesi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyStyleWithRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            
            // Kaynak aralığa bazı örnek stiller ekleyin
            Cells cellsSrc = sheetSrc.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A1:D5");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            rangeSrc.SetStyle(style);
            
            // Hedef çalışma sayfasını oluştur
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";
            
            // Hedef aralığı oluştur ve stili kopyala
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange("A1:D5");
            rangeDest.CopyStyle(rangeSrc);
            
            // Çalışma kitabını kaydedin
            workbook.Save("RangeCopyStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


