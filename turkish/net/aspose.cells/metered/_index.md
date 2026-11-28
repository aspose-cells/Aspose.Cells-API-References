---
title: "Metered sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Metered sınıfı. Metered anahtarını ayarlamak için yöntemler sağlar"
type: docs
url: /tr/net/aspose.cells/metered/
---
## Metered class

Ölçülü anahtarı ayarlamak için yöntemler sağlar.

```csharp
public class Metered
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Metered](metered/)() | Bu sınıfın yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetProductName](../../aspose.cells/metered/getproductname/)() | Ürün adını alır |
| [SetMeteredKey](../../aspose.cells/metered/setmeteredkey/)(string, string) | Metered public ve private anahtarını ayarlar. Metered lisansı satın alırsanız, uygulamayı başlattığınızda bu API çağrılmalıdır, genellikle bu yeterlidir. Ancak, tüketim verileri yüklenemeyip 24 saati aşarsa, lisans değerlendirme durumuna ayarlanır; böyle bir durumu önlemek için lisans durumunu düzenli olarak kontrol etmelisiniz, eğer değerlendirme durumundaysa, bu API'yi tekrar çağırın. |
| static [GetConsumptionCredit](../../aspose.cells/metered/getconsumptioncredit/)() | Tüketim kredisini alır |
| static [GetConsumptionQuantity](../../aspose.cells/metered/getconsumptionquantity/)() | Tüketim dosya boyutunu alır |
| static [IsMeteredLicensed](../../aspose.cells/metered/ismeteredlicensed/)() | Metered'in lisanslı olup olmadığını kontrol et |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredDemo
    {
        public static void MeteredExample()
        {
            // Metered sınıfının bir örneğini oluştur
            Metered metered = new Metered();

            // Metered anahtarını ayarla
            string publicKey = "YourPublicKey";
            string privateKey = "YourPrivateKey";
            metered.SetMeteredKey(publicKey, privateKey);

            // Ürün adını al ve göster
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Örneğin, bir çalışma kitabı oluşturup kaydetmek için ek kod
            // Örneğin, bir çalışma kitabı oluşturup kaydetmek
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            workbook.Save("MeteredExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


