---
title: "BuiltInDocumentPropertyCollection.HyperlinkBase"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. hyperlinkbase özelliğini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/hyperlinkbase/
---
## BuiltInDocumentPropertyCollection.HyperlinkBase property

hyperlinkbase özelliğini alır veya ayarlar.

```csharp
public string HyperlinkBase { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyHyperlinkBaseDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // HyperlinkBase özelliğini ayarlayın
            workbook.BuiltInDocumentProperties.HyperlinkBase = "http://www.example.com";

            // Demonstrasyon için başka bir özelliği ayarlayın
            workbook.BuiltInDocumentProperties.Title = "Sample Workbook";

            // Çalışma kitabını kaydedin
            workbook.Save("HyperlinkBaseDemo.xlsx", SaveFormat.Xlsx);

            // Kaydedilmiş çalışma kitabını yükleyerek özellikleri doğrulayın
            Workbook loadedWorkbook = new Workbook("HyperlinkBaseDemo.xlsx");
            
            // Özellikleri konsola çıktı olarak verin
            Console.WriteLine("HyperlinkBase: " + loadedWorkbook.BuiltInDocumentProperties.HyperlinkBase);
            Console.WriteLine("Title: " + loadedWorkbook.BuiltInDocumentProperties.Title);
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


