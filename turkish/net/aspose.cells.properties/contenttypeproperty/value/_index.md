---
title: "ContentTypeProperty.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ContentTypeProperty özelliği. İçerik türü özelliğinin değerini döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/contenttypeproperty/value/
---
## ContentTypeProperty.Value property

İçerik türü özelliğinin değerini döndürür veya ayarlar.

```csharp
public string Value { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Bir içerik türü özelliği ekle
            workbook.ContentTypeProperties.Add("Admin", "InitialValue", "text");
            
            // Özelliğin Değerine eriş ve değiştir
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.Value = "Aspose"; // Demonstrating Value property usage
            
            // Çalışma kitabını kaydedin
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


