---
title: "Sınıf CustomProperty"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Properties.CustomProperty sınıfı. Çalışma sayfası için kullanıcı tanımlı rastgele verilerin ad ve değer çiftlerini depolayan bir özel özelliği temsil eder"
type: docs
url: /tr/net/aspose.cells.properties/customproperty/
---
## CustomProperty class

Çalışma sayfası için kullanıcı tarafından tanımlanan rastgele verilerin ad ve değer çiftlerini depolayan bir özel özelliği temsil eder.

```csharp
public class CustomProperty
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BinaryValue](../../aspose.cells.properties/customproperty/binaryvalue/) { get; set; } | Özel özelliğin ikili değerini alır ve ayarlar. |
| [Name](../../aspose.cells.properties/customproperty/name/) { get; set; } | Nesnenin adını döndürür veya ayarlar. |
| [StringValue](../../aspose.cells.properties/customproperty/stringvalue/) { get; set; } | (**Obsolete.**) Özel özelliğin değerini alır veya ayarlar. |
| [Value](../../aspose.cells.properties/customproperty/value/) { get; set; } | Özel özelliğin değerini döndürür veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyDemo
    {
        public static void CustomPropertyExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // CustomProperties koleksiyonuna eriş
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // Özel özellikler ekle
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("LastModified", DateTime.Now.ToString());

            // Özel özelliklere eriş ve görüntüle
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CustomPropertyExample.xlsx");
            workbook.Save("CustomPropertyExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


