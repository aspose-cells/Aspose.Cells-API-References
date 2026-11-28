---
title: "CustomProperty.BinaryValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomProperty özelliği. Özel özelliğin ikili değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/customproperty/binaryvalue/
---
## CustomProperty.BinaryValue property

Özel özelliğin ikili değerini alır ve ayarlar.

```csharp
public byte[] BinaryValue { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyBinaryValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek bir değerle özel bir özellik ekleyin
            worksheet.CustomProperties.Add("SampleBinary", "01010101");

            try
            {
                // Özel özelliği al
                CustomProperty prop = worksheet.CustomProperties["SampleBinary"];

                // Özel özelliğin Adını ve Değerini görüntüleyin
                Console.WriteLine($"Custom Property Name : {prop.Name}");
                Console.WriteLine($"Custom Property Value: {prop.Value}");

                // NOT: CustomProperty yansıtması BinaryValue özelliğini içermez.
                // Kullanılabilir metin tabanlı değere 'Value' özelliği aracılığıyla erişilir.

                // Çalışma kitabını kaydedin (isteğe bağlı)
                workbook.Save("BinaryValueDemo.xlsx");
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


