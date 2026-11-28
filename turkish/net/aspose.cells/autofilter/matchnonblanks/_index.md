---
title: "AutoFilter.MatchNonBlanks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Listedeki boş olmayan tüm hücreleri eşleştir"
type: docs
url: /tr/net/aspose.cells/autofilter/matchnonblanks/
---
## AutoFilter.MatchNonBlanks method

Listedeki tüm boş olmayan hücreleri eşleştir.

```csharp
public void MatchNonBlanks(int fieldIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | Int32 | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan field 0'dır). |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodMatchNonBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı boş hücreler içeren örnek veri ekle
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(""); // Blank cell
            worksheet.Cells["B3"].PutValue(5);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(8);
            worksheet.Cells["A5"].PutValue(""); // Blank cell
            worksheet.Cells["B5"].PutValue(12);

            // A sütununda (indeks 0) sadece boş olmayan hücreleri göstermek için otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.MatchNonBlanks(0);
            worksheet.AutoFilter.Refresh();

            // Çalışma kitabını kaydedin
            workbook.Save("FilterNonBlanks.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


