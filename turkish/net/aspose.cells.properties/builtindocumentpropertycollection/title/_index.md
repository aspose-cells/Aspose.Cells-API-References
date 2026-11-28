---
title: "BuiltInDocumentPropertyCollection.Title"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Belgenin başlığını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/title/
---
## BuiltInDocumentPropertyCollection.Title property

Belgenin başlığını alır veya ayarlar.

```csharp
public string Title { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTitleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Title özelliğini ayarla
            workbook.BuiltInDocumentProperties.Title = "Sample Document Title";
            
            // Title özelliğini göster
            Console.WriteLine("Document Title: " + workbook.BuiltInDocumentProperties.Title);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


