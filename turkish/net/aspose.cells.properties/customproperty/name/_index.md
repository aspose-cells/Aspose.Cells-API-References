---
title: "CustomProperty.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomProperty özelliği. Nesnenin adını döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

Nesnenin adını döndürür veya ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Adı ve değeri olan bir özel özellik ekleyin
                worksheet.CustomProperties.Add("SampleName", "SampleValue");

                // Özel özelliği al
                CustomProperty customProperty = worksheet.CustomProperties["SampleName"];

                // Name özelliğinin mevcut değerini görüntüleyin (okuma işlemi)
                Console.WriteLine("Custom Property Name: " + customProperty.Name);

                // Name özelliği için yeni bir değer ayarlayın
                customProperty.Name = "UpdatedName";
                Console.WriteLine("Updated Custom Property Name: " + customProperty.Name);

                // Çalışma kitabını kaydedin
                workbook.Save("NameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


