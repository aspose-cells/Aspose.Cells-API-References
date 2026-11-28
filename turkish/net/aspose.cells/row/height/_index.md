---
title: "Row.Height"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Satır özelliği. Satır yüksekliğini puan biriminde alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/row/height/
---
## Row.Height property

Satır yüksekliğini Nokta biriminde alır ve ayarlar.

```csharp
public double Height { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyHeightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk satır için satır yüksekliğini ayarlayın
            Row row = worksheet.Cells.Rows[0];
            row.Height = 30;
            
            // Satıra bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Row with custom height");
            
            // Satır yüksekliğini doğrulayın ve görüntüleyin
            Console.WriteLine("Row 1 Height: " + row.Height);
            
            // Çalışma kitabını kaydedin
            workbook.Save("RowHeightDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


