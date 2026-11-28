---
title: "Enum PropertyType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Properties.PropertyType enum. Bir belge özelliğinin veri tipini belirtir"
type: docs
url: /tr/net/aspose.cells.properties/propertytype/
---
## PropertyType enumeration

Bir belge özelliğinin veri tipini belirtir.

```csharp
public enum PropertyType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Boolean | `0` | Özellik bir boolean değerdir. |
| DateTime | `1` | Özellik bir tarih saat değeridir. |
| Double | `2` | Özellik bir kayan nokta sayıdır. |
| Number | `3` | Özellik bir tam sayı değeridir. |
| String | `4` | Özellik bir metin değeridir. |
| Blob | `5` | Özellik bir bayt dizisidir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class PropertyTypeDemo
    {
        public static void PropertyTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yerleşik belge özelliklerine eriş
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Bazı yerleşik özellikleri ayarla
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demonstration of PropertyType";
            builtInProperties.Company = "Aspose";

            // Özel belge özelliklerine eriş
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Farklı tiplerde özel özellikler ekle
            customProperties.Add("IsReviewed", true); // Boolean
            customProperties.Add("ReviewDate", DateTime.Now); // DateTime
            customProperties.Add("Rating", 4.5); // Double
            customProperties.Add("Pages", 100); // Number
            customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String

            // Özel özellikleri al ve görüntüle
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("PropertyTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


