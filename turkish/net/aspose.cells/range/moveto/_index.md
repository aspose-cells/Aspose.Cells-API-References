---
title: "Range.MoveTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Geçerli aralığı hedef aralığa taşı"
type: docs
url: /tr/net/aspose.cells/range/moveto/
---
## Range.MoveTo method

Geçerli aralığı hedef aralığa taşı.

```csharp
public void MoveTo(int destRow, int destColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destRow | Int32 | Hedef aralığın başlangıç satırı. |
| destColumn | Int32 | Hedef aralığın başlangıç sütunu. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek bir aralık oluştur (A1:B2)
            Aspose.Cells.Range originalRange = worksheet.Cells.CreateRange("A1", "B2");
            
            // Gösterim için aralığa bazı veriler koy
            originalRange[0, 0].PutValue("A1");
            originalRange[0, 1].PutValue("B1");
            originalRange[1, 0].PutValue("A2");
            originalRange[1, 1].PutValue("B2");
            
            // Aralığı 1 satır aşağı kaydır (A2:B3'e)
            originalRange.MoveTo(originalRange.FirstRow + 1, originalRange.FirstColumn);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


