---
title: "BuiltInDocumentPropertyCollection.LastPrinted"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Belgenin en son yerel saat diliminde yazdırıldığı tarihi alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinted/
---
## BuiltInDocumentPropertyCollection.LastPrinted property

Belgenin son kez yerel saat diliminde yazdırıldığı tarihi alır veya ayarlar.

```csharp
public DateTime LastPrinted { get; set; }
```

### Açıklamalar

Belge hiç yazdırılmadıysa, bu özellik DateTime.MinValue değerini döndürür.

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yerleşik belge özelliklerini ayarlayın
            workbook.BuiltInDocumentProperties.CreatedTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now.AddDays(-1); // Set to yesterday
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // LastPrinted özelliğini göster
            Console.WriteLine("Last printed: " + workbook.BuiltInDocumentProperties.LastPrinted);

            // Çalışma kitabını kaydedin
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


