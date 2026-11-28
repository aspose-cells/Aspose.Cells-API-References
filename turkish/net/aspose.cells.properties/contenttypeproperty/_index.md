---
title: "Sınıf ContentTypeProperty"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Properties.ContentTypeProperty sınıfı. Tanımlayıcı bilgileri temsil eder"
type: docs
url: /tr/net/aspose.cells.properties/contenttypeproperty/
---
## ContentTypeProperty class

Tanımlayıcı bilgileri temsil eder.

```csharp
public class ContentTypeProperty
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IsNillable](../../aspose.cells.properties/contenttypeproperty/isnillable/) { get; set; } | Değerin boş olabileceğini gösterir. |
| [Name](../../aspose.cells.properties/contenttypeproperty/name/) { get; set; } | Nesnenin adını döndürür veya ayarlar. |
| [Type](../../aspose.cells.properties/contenttypeproperty/type/) { get; set; } | Özelliğin tipini alır ve ayarlar. |
| [Value](../../aspose.cells.properties/contenttypeproperty/value/) { get; set; } | İçerik türü özelliğinin değerini döndürür veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class ContentTypePropertyDemo
    {
        public static void ContentTypePropertyExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // Yeni bir içerik türü özelliği ekle
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Yeni eklenen özelliğe eriş
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Özellikleri ayarlama
            property.Name = "Admin";
            property.Value = "Aspose";
            property.Type = "text";
            property.IsNillable = true;

            // Excel dosyasını kaydet
            workbook.Save("ContentTypePropertyExample.xlsx");
            workbook.Save("ContentTypePropertyExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


