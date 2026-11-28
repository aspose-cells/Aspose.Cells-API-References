---
title: "Range.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Aralığın adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/range/name/
---
## Range.Name property

Aralığın adını alır veya ayarlar.

```csharp
public string Name { get; set; }
```

### Açıklamalar

Adlandırılmış aralık desteklenir. Örneğin,

range.Name = "Sheet1!MyRange";

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir aralık oluşturun (A sütunundan B sütununa kadar)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, true);
            
            // Aralık için ad özelliğini ayarlayın
            range.Name = "testRange";
            
            // Adın ayarlandığını doğrulayın
            Console.WriteLine("Range name: " + range.Name);
            
            // Çalışma kitabını kaydedin
            workbook.Save("RangeWithName.xlsx");
            
            // Adın kalıcı olduğunu göstermek için kaydedilmiş dosyayı açın
            Workbook loadedWorkbook = new Workbook("RangeWithName.xlsx");
            Aspose.Cells.Range loadedRange = loadedWorkbook.Worksheets[0].Cells.CreateRange(0, 2, true);
            Console.WriteLine("Loaded range name: " + loadedRange.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


