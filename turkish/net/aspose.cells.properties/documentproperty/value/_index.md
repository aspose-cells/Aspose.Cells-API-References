---
title: "DocumentProperty.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentProperty özelliği. Özelliğin değerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/documentproperty/value/
---
## DocumentProperty.Value property

Özelliğin değerini alır veya ayarlar.

```csharp
public object Value { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yerleşik belge özelliklerine eriş
            var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
            hyperlinkBase.Value = "http://www.example.com";

            var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            title.Value = "Sample Document Title";

            // Çalışma kitabını kaydedin
            workbook.Save("DocumentPropertiesDemo.xlsx");

            // Ayarlanan değerleri göster
            Console.WriteLine("HyperlinkBase: " + hyperlinkBase.Value);
            Console.WriteLine("Title: " + title.Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


