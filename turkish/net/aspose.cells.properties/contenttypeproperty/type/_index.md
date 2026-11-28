---
title: "ContentTypeProperty.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ContentTypeProperty özelliği. Özelliğin tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/contenttypeproperty/type/
---
## ContentTypeProperty.Type property

Özelliğin tipini alır ve ayarlar.

```csharp
public string Type { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Farklı tiplerde içerik türü özellikleri ekle
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            workbook.ContentTypeProperties.Add("Version", "1.0", "number");
            workbook.ContentTypeProperties.Add("Enabled", "true", "boolean");

            // Özellik tiplerine eriş ve göster
            foreach (ContentTypeProperty property in workbook.ContentTypeProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

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


