---
title: "CellsHelper.SignificantDigits"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper özelliği. Önemli basamak sayısını alır ve ayarlar. Varsayılan değer 17'dir"
type: docs
url: /tr/net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

Önemli basamak sayısını alır ve ayarlar. Varsayılan değer 17'dir.

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static int SignificantDigits { get; set; }
```

### Açıklamalar

Şu anda sadece 15 veya 17 olabilir. NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [`SignificantDigitsType`](../significantdigitstype/) kullanın. Bu özellik, Haziran 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Önemli basamakları ayarla
            CellsHelper.SignificantDigits = 15;
            
            // Özelliğin kullanımını göster
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            
            // Hesaplamalarda önemli basamakları göstermek için bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Önemli basamaklardan etkilenecek değerleri ayarla
            worksheet.Cells["A1"].PutValue(1.2345678912345678);
            worksheet.Cells["A2"].PutValue(1.2345678912345678);
            worksheet.Cells["A3"].Formula = "=A1+A2";
            
            // Ayarlanan önemli basamaklarla formülleri hesapla
            workbook.CalculateFormula();
            
            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Value with significant digits: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


