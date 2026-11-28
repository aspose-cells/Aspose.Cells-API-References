---
title: "BuiltInDocumentPropertyCollection.LinksUpToDate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Bir belgedeki hiperlinklerin güncel olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/linksuptodate/
---
## BuiltInDocumentPropertyCollection.LinksUpToDate property

Bir belgedeki hiperlinklerin güncel olup olmadığını gösterir.

```csharp
public bool LinksUpToDate { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLinksUpToDateDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yerleşik belge özellikleri koleksiyonuna erişin
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // LinksUpToDate özelliğini, hiperlinklerin güncel olup olmadığını gösterecek şekilde ayarla
            builtInProperties.LinksUpToDate = true;

            // Özelliği göstermek için basit bir hiperlink ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Çalışma kitabını kaydedin
            workbook.Save("LinksUpToDateDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


