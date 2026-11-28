---
title: "Range.CopyValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Bir kaynak aralıktan hücre değerini kopyalar"
type: docs
url: /tr/net/aspose.cells/range/copyvalue/
---
## Range.CopyValue method

Kaynak bir aralıktan hücre değerini kopyalar.

```csharp
public void CopyValue(Range range)
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
    public class RangeMethodCopyValueWithRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle ve ilk çalışma sayfasını al
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "SourceSheet";
            
            // Hedef için başka bir çalışma sayfası ekle
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "DestinationSheet";
            
            // Kaynak aralıkta örnek veri oluştur
            Cells cellsSrc = sheetSrc.Cells;
            cellsSrc["A1"].PutValue("Source Data");
            cellsSrc["A2"].PutValue(10);
            cellsSrc["B2"].PutValue(20);
            cellsSrc["A3"].PutValue(30);
            cellsSrc["B3"].PutValue(40);
            
            // Kaynak ve hedef için aralıklar oluştur
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A2:B3");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("D2:E3");
            
            // Kaynak aralıktan hedef aralığa değerleri kopyala
            rangeDest.CopyValue(rangeSrc);
            
            // Çalışma kitabını kaydedin
            workbook.Save("RangeCopyValueDemo.xlsx");
            
            Console.WriteLine("Values copied successfully from source range to destination range.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


