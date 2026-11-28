---
title: "Metered.GetConsumptionQuantity"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Metered yöntemi. Tüketim dosya boyutunu alır"
type: docs
url: /tr/net/aspose.cells/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Tüketim dosya boyutunu alır

```csharp
public static decimal GetConsumptionQuantity()
```

### Dönüş Değeri

tüketim miktarı

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionQuantityDemo
    {
        public static void Run()
        {
            // Bir metered örneği oluşturun
            Metered metered = new Metered();

            try
            {
                // Ölçülen anahtarları ayarla (gerçek kullanımda gerçek anahtarlarla değiştir)
                metered.SetMeteredKey("your-public-key", "your-private-key");

                // Tüketim miktarını al
                decimal consumptionQuantity = Metered.GetConsumptionQuantity();

                // Sonucu göster
                Console.WriteLine($"Consumption Quantity: {consumptionQuantity}");

                // Ölçülen kullanımı göstermek için bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Çalışma kitabının işlevsel olduğunu göstermek için bazı veriler ekle
                worksheet.Cells["A1"].PutValue("Metered Consumption Demo");
                worksheet.Cells["A2"].PutValue($"Consumption Quantity: {consumptionQuantity}");

                // Çalışma kitabını kaydedin
                workbook.Save("MeteredConsumptionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in metered operation: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


