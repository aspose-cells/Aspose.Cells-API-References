---
title: "CustomProperty.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomProperty özelliği. Özel özelliğin değerini döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/customproperty/value/
---
## CustomProperty.Value property

Özel özelliğin değerini döndürür veya ayarlar.

```csharp
public string Value { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Uzun bir dize değeriyle bir özel özellik ekle
            worksheet.CustomProperties.Add("VeryLongString", "This is a very long string value for testing custom properties");
            
            // Özel özelliğin değerini al ve görüntüle
            string propertyValue = worksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Custom Property Value: " + propertyValue);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Özelliğin kalıcı olduğunu doğrulamak için çalışma kitabını yeniden yükle
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Yükleme sonrası değerin aynı olduğunu doğrula
            string loadedValue = loadedWorksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Reloaded Custom Property Value: " + loadedValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


