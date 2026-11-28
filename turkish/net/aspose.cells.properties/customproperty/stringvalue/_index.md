---
title: "CustomProperty.StringValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomProperty özelliği. Özel özelliğin değerini döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/customproperty/stringvalue/
---
## CustomProperty.StringValue property

Özel özelliğin değerini döndürür veya ayarlar.

```csharp
[Obsolete("Use CustomProperty.Value property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValue { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen CustomProperty.Value özelliğini kullanın. Bu özellik, Haziran 2010'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyStringValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Dize değeriyle bir özel özellik ekle
                worksheet.CustomProperties.Add("SampleProperty", "Test Value");

                // Özel özelliği al
                CustomProperty customProperty = worksheet.CustomProperties["SampleProperty"];

                // StringValue özelliğini görüntüle (okuma işlemi)
                Console.WriteLine("StringValue: " + customProperty.StringValue);

                // StringValue özelliği için yeni bir değer ayarla
                customProperty.StringValue = "Updated Value";
                Console.WriteLine("Updated StringValue: " + customProperty.StringValue);

                // Çalışma kitabını kaydedin
                workbook.Save("StringValueDemo.xlsx");
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


