---
title: "Metered.GetConsumptionCredit"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Metered yöntemi. Tüketim kredisini alır"
type: docs
url: /tr/net/aspose.cells/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

Tüketim kredisini alır

```csharp
public static decimal GetConsumptionCredit()
```

### Dönüş Değeri

tüketim miktarı

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionCreditDemo
    {
        public static void Run()
        {
            // Metered sınıfının bir örneğini oluştur
            Metered metered = new Metered();

            try
            {
                // GetConsumptionCredit yöntemini statik olarak çağır
                decimal consumptionCredit = Metered.GetConsumptionCredit();
                
                // Sonucu göster
                Console.WriteLine($"Current consumption credit: {consumptionCredit}");
                
                // Etkiyi göstermek için basit bir çalışma kitabı oluştur (ancak GetConsumptionCredit çalışma kitabını değiştirmez)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Tüketim kredi bilgilerini çalışma sayfasına ekle
                worksheet.Cells["A1"].PutValue("Consumption Credit:");
                worksheet.Cells["B1"].PutValue(consumptionCredit.ToString());
                
                // Çalışma kitabını kaydedin
                workbook.Save("MeteredGetConsumptionCreditDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error getting consumption credit: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


