---
title: "BuiltInDocumentPropertyCollection.ContentStatus"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Belgenin içerik durumunu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/contentstatus/
---
## BuiltInDocumentPropertyCollection.ContentStatus property

Belgenin içerik durumunu alır veya ayarlar.

```csharp
public string ContentStatus { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentStatusDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // ContentStatus dahil yerleşik belge özelliklerini ayarlayın
            workbook.BuiltInDocumentProperties.ContentStatus = "Draft";
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";

            // Çalışma kitabını kaydedin
            workbook.Save("DocumentWithContentStatus.xlsx", SaveFormat.Xlsx);

            // Kaydedilmiş çalışma kitabını yükleyerek özellikleri doğrulayın
            Workbook loadedWorkbook = new Workbook("DocumentWithContentStatus.xlsx");
            
            // ContentStatus özelliğini görüntüleyin
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


