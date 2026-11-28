---
title: "BuiltInDocumentPropertyCollection.Template"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Belge şablonunun bilgilendirici adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/template/
---
## BuiltInDocumentPropertyCollection.Template property

Belge şablonunun bilgi adını alır veya ayarlar.

```csharp
public string Template { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTemplateDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yerleşik belge özelliklerine eriş
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Template özelliğini ayarla
            builtInProperties.Template = "Standard Template";

            // Demonstrasyon için diğer temel özellikleri ayarla
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Template Property Demo";

            // Çalışma kitabını kaydedin
            workbook.Save("TemplatePropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


