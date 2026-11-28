---
title: "TxtLoadOptions.IsMultiEncoded"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. True, dosyanın birden fazla kodlama içerdiği anlamına gelir"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/ismultiencoded/
---
## TxtLoadOptions.IsMultiEncoded property

True, dosyanın birden fazla kodlama içerdiği anlamına gelir.

```csharp
public bool IsMultiEncoded { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyIsMultiEncodedDemo
    {
        public static void Run()
        {
            // Metin yükleme seçeneklerini oluşturun
            TxtLoadOptions options = new TxtLoadOptions();
            
            // Birden fazla kodlamayı işlemek için IsMultiEncoded'i true olarak ayarlayın
            options.IsMultiEncoded = true;
            
            // Çalışma kitabını seçeneklerle yükleyin
            Workbook workbook = new Workbook("example.csv", options);
            
            // Yüklenen dosyadan örnek değerleri göster
            Console.WriteLine("A2 Cell Value: " + workbook.Worksheets[0].Cells["A2"].StringValue);
            Console.WriteLine("A3 Cell Value: " + workbook.Worksheets[0].Cells["A3"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


