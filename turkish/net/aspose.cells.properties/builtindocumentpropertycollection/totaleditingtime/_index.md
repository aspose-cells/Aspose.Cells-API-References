---
title: "BuiltInDocumentPropertyCollection.TotalEditingTime"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Toplam düzenleme süresini dakikalar cinsinden alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/totaleditingtime/
---
## BuiltInDocumentPropertyCollection.TotalEditingTime property

Toplam düzenleme süresini dakikalar cinsinden alır veya ayarlar.

```csharp
public double TotalEditingTime { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTotalEditingTimeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yerleşik belge özelliklerine eriş
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Toplam düzenleme süresini dakikalar cinsinden ayarla
            builtInProperties.TotalEditingTime = 90.5;

            // Ayarlanan düzenleme süresini göster
            Console.WriteLine("Total Editing Time: " + builtInProperties.TotalEditingTime + " minutes");

            // Çalışma kitabını kaydedin
            workbook.Save("TotalEditingTimeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


