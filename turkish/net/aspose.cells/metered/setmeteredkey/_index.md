---
title: "Metered.SetMeteredKey"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Metered yöntemi. Metered genel ve özel anahtarı ayarlar. Uygulamayı başlattığınızda metered lisansı satın alırsanız bu API normal olarak çağrılmalıdır, bu yeterlidir. Ancak tüketim verilerini yükleme sürekli başarısız olur ve 24 saati aşarsa lisans değerlendirme durumuna ayarlanır; böyle bir durumu önlemek için lisans durumunu düzenli olarak kontrol etmeli ve eğer değerlendirme durumundaysa bu API'yi tekrar çağırmalısınız."
type: docs
url: /tr/net/aspose.cells/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Metered public ve private anahtarını ayarlar. Metered lisansı satın alırsanız, uygulamayı başlattığınızda bu API çağrılmalıdır, genellikle bu yeterlidir. Ancak, tüketim verileri yüklenemeyip 24 saati aşarsa, lisans değerlendirme durumuna ayarlanır; böyle bir durumu önlemek için lisans durumunu düzenli olarak kontrol etmelisiniz, eğer değerlendirme durumundaysa, bu API'yi tekrar çağırın.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| publicKey | String | açık anahtar |
| privateKey | String | özel anahtar |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodSetMeteredKeyWithStringStringDemo
    {
        public static void Run()
        {
            // Ölçülen genel ve özel anahtarları ayarla
            Metered metered = new Metered();
            metered.SetMeteredKey(
                "asposenet7c90badb00ba4f4bbd35634f4d481c14",
                "FBJnGi61yW8meqVfugVpqX5WXyBIgDOp-XaEV5MjzuABC9OKu6SwMP00KWZo8ULVfvkYPG4thnNerNPvvRohz1hAMjG9SkQ4akclON6VqBdXuxbasF1aXwShbIBNTA7Ac*3OnFxDo4jcvg0XyTSyQjA*vxhq*0YEr2MgedtncGUiCyC7o775f7uXusxe*UWVDdI*qNzEdSU*f7Sl6a9qiDBAA*q2OrXbd9jOAgiP1TiAq6vluG7vqK-dKZlTOmL*A-Uo0rxU73ZjtYW*TLZAW2jTbzVIOHyws3l6DF5G98ayvKt1iye5ce4HNkvxwk3*uNyMd-JQeGz64hQpjU5Cdw__");

            // Ölçülen tüketim miktarını al
            decimal consumption = Metered.GetConsumptionQuantity();
            Console.WriteLine("Consumption quantity: " + consumption);

            // Ölçülen tüketim kredisini al
            decimal credit = Metered.GetConsumptionCredit();
            Console.WriteLine("Consumption credit: " + credit);
        }
    }
}
```

### Ayrıca Bakınız

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


