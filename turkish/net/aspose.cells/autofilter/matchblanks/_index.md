---
title: "AutoFilter.MatchBlanks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Listedeki tüm boş hücreleri eşleştir"
type: docs
url: /tr/net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

Listedeki tüm boş hücreleri eşleştir.

```csharp
public void MatchBlanks(int fieldIndex)
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
    public class AutoFilterMethodMatchBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı boş hücreler içeren örnek veri ekle
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // C2'yi boş bırak
            
            worksheet.Cells["A3"].PutValue("Data3");
            // B3'ü boş bırak
            worksheet.Cells["C3"].PutValue("Data6");
            
            // Otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:C3";
            AutoFilter filter = worksheet.AutoFilter;
            
            // 3. sütunda (C) boş hücreleri içeren satırları sadece gösterecek şekilde filtrele
            filter.MatchBlanks(2); // Column index is 0-based
            
            // Filtreyi yenile
            filter.Refresh();
            
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFilterMatchBlanksDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


