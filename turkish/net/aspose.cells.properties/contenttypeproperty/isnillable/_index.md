---
title: "ContentTypeProperty.IsNillable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ContentTypeProperty özelliği. Değerin boş olabileceğini gösterir"
type: docs
url: /tr/net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

Değerin boş olabileceğini gösterir.

```csharp
public bool IsNillable { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyIsNillableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Bir içerik türü özelliği ekle
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Özelliğe eriş ve IsNillable'ı ayarla
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.IsNillable = true;
            
            // IsNillable değerini doğrula ve çıktı al
            Console.WriteLine($"Property 'Admin' IsNillable: {property.IsNillable}");
            
            workbook.Save("ContentTypePropertyIsNillableDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


