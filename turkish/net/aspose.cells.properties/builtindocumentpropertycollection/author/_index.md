---
title: "BuiltInDocumentPropertyCollection.Author"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Belgenin yazarının adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/author/
---
## BuiltInDocumentPropertyCollection.Author property

Belgenin yazarının adını alır veya ayarlar.

```csharp
public string Author { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyAuthorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yazar özelliğini ayarla
            string authorName = "John Doe";
            workbook.BuiltInDocumentProperties.Author = authorName;

            // Yazar özelliğini görüntüleyin
            Console.WriteLine("Document Author: " + workbook.BuiltInDocumentProperties.Author);

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


