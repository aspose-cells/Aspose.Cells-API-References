---
title: "Worksheet.CustomProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Çalışma sayfası özelliği. Bir çalışma sayfasıyla ilişkili tanımlayıcı bilgileri temsil eden bir nesne alır."
type: docs
url: /tr/net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

Bir çalışma sayfasıyla ilişkili tanımlayıcı bilgilerini temsil eden nesneyi alır.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### Açıklamalar

Worksheet.CustomProperties, rastgele veri depolamak için tercih edilen bir mekanizma sağlar. Eski üçüncü taraf belge bileşenlerini ve ikili parçalara sıkı bir ihtiyaç duyulan durumları da destekler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCustomPropertiesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına özel özellikler ekle
            worksheet.CustomProperties.Add("Property1", "Value1");
            worksheet.CustomProperties.Add("Property2", "12345");
            worksheet.CustomProperties.Add("Property3", DateTime.Now.ToString());
            
            // Özel özelliklerin sayısını göster
            Console.WriteLine("Custom Properties Count: " + worksheet.CustomProperties.Count);
            
            // Özellik değerlerine eriş ve göster
            foreach (var prop in worksheet.CustomProperties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetCustomPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


