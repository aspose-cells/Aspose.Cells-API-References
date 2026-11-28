---
title: "BuiltInDocumentPropertyCollection.Keywords"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Belge anahtar kelimelerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/keywords/
---
## BuiltInDocumentPropertyCollection.Keywords property

Belge anahtar kelimelerini alır veya ayarlar.

```csharp
public string Keywords { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyKeywordsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Keywords özelliğini ayarla
            workbook.BuiltInDocumentProperties.Keywords = "Sample Keywords, Aspose.Cells, Demo";
            
            // Çalışma kitabını kaydedin
            workbook.Save("output_keywords.xlsx");
            
            // Kaydedilmiş çalışma kitabını yükleyerek Keywords özelliğini doğrula
            Workbook loadedWorkbook = new Workbook("output_keywords.xlsx");
            
            // Keywords özelliğini göster
            Console.WriteLine("Document Keywords: " + loadedWorkbook.BuiltInDocumentProperties.Keywords);
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


