---
title: "Metered.IsMeteredLicensed"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Metered yöntemi. Metered'in lisanslı olup olmadığını kontrol edin"
type: docs
url: /tr/net/aspose.cells/metered/ismeteredlicensed/
---
## Metered.IsMeteredLicensed method

Metered'in lisanslı olup olmadığını kontrol et

```csharp
public static bool IsMeteredLicensed()
```

### Dönüş Değeri

Doğru veya yanlış

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodIsMeteredLicensedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir Metered örneği oluşturun
            Metered metered = new Metered();

            try
            {
                // Metered lisansının uygulanıp uygulanmadığını kontrol edin
                bool isLicensed = Metered.IsMeteredLicensed();

                // Sonucu göster
                Console.WriteLine($"Is Metered Licensed: {isLicensed}");

                // Sonucu çalışma sayfasına ekleyin
                worksheet.Cells["A1"].PutValue("Is Metered Licensed:");
                worksheet.Cells["B1"].PutValue(isLicensed);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsMeteredLicensed method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("MethodIsMeteredLicensedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


