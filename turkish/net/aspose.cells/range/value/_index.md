---
title: "Range.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Aralığın değerini alır ve ayarlar."
type: docs
url: /tr/net/aspose.cells/range/value/
---
## Range.Value property

Aralığın değerini alır ve ayarlar.

```csharp
public object Value { get; set; }
```

### Açıklamalar

Aralık birden fazla hücre içeriyorsa, döndürülen/uygulanan nesne iki boyutlu bir Dizi nesnesi olmalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1'den başlayan ve 3x3 hücreyi kapsayan bir aralık oluştur.
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");

            // Aralık için değeri 2B bir dizi olarak ayarla.
            int[,] values = new int[3, 3] { { 1, 2, 3 }, { 4, 5, 6 }, { 7, 8, 9 } };
            range.Value = values;

            // Çalışma kitabını kaydedin
            workbook.Save("RangePropertyValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


