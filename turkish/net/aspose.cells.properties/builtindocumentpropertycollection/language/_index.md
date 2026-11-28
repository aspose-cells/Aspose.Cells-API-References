---
title: "BuiltInDocumentPropertyCollection.Language"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Belgenin dilini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/language/
---
## BuiltInDocumentPropertyCollection.Language property

Belgenin dilini alır veya ayarlar.

```csharp
public string Language { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLanguageDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yerleşik belge özellikleri koleksiyonuna erişin
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // language özelliğini ayarla
            builtInProperties.Language = "en-US";

            // Demonstrasyon için diğer temel özellikleri ayarla
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Language Property Demo";

            // Çalışma kitabını kaydedin
            workbook.Save("LanguagePropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


