---
title: "Range.EntireRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Belirtilen aralığı içeren tüm satırı veya satırları temsil eden bir Range nesnesi alır"
type: docs
url: /tr/net/aspose.cells/range/entirerow/
---
## Range.EntireRow property

Belirtilen aralığı içeren tüm satırı (veya satırları) temsil eden bir Range nesnesi alır.

```csharp
public Range EntireRow { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // İlk satıra bazı örnek veriler ekleyin
            for (int col = 0; col < 5; col++)
            {
                sheet.Cells[0, col].PutValue($"Header {col + 1}");
            }

            // EntireRow özelliğini kullanarak tüm ilk satırı alın
            Aspose.Cells.Range entireRow = sheet.Cells.CreateRange("A1").EntireRow;

            // İlk satırı üçüncü satıra kopyalayın
            Aspose.Cells.Range destination = sheet.Cells.CreateRange("A3").EntireRow;
            destination.Copy(entireRow);

            // Çalışma kitabını kaydedin
            workbook.Save("EntireRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


