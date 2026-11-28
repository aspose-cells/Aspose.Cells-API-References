---
title: "Cell.Formula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrenin formülünü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cell/formula/
---
## Cell.Formula property

[`Cell`](../) formülünü alır veya ayarlar

```csharp
public string Formula { get; set; }
```

### Açıklamalar

Bir formül dizesi her zaman eşittir işareti (=) ile başlar. Ve lütfen parametre ayırıcı olarak her zaman virgül (,) kullanın, örneğin "=SUM(A1, E1, H2)".

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Formülde kullanılacak hücrelerdeki değerleri ayarlayın
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A1"].PutValue(100);

            // B6 hücresine formülü ayarlayın
            worksheet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + A1";

            // Formülü hesapla
            workbook.CalculateFormula();

            // Sonucu göster
            Console.WriteLine("Formula result in B6: " + worksheet.Cells["B6"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


