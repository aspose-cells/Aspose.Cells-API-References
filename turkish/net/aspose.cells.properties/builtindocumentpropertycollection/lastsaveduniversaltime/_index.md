---
title: "BuiltInDocumentPropertyCollection.LastSavedUniversalTime"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Son kaydetmenin evrensel zamanını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/lastsaveduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastSavedUniversalTime property

Son kaydetmenin evrensel zamanını alır veya ayarlar.

```csharp
public DateTime LastSavedUniversalTime { get; set; }
```

### Açıklamalar

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedUniversalTimeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yerleşik belge özelliklerine eriş
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // LastSavedUniversalTime özelliğini ayarla
            DateTime utcNow = DateTime.UtcNow;
            builtInProperties.LastSavedUniversalTime = utcNow;

            // Ayarlanan değeri görüntüleyin
            Console.WriteLine("LastSavedUniversalTime set to: " + builtInProperties.LastSavedUniversalTime);

            // Çalışma kitabını kaydedin
            workbook.Save("LastSavedUniversalTimeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


