---
title: "Enum AccessCacheOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AccessCacheOptions enum. Veri erişimi için önbellekleme seçenekleri. Birden fazla seçenek,  operatörü kullanılarak birleştirilebilir"
type: docs
url: /tr/net/aspose.cells/accesscacheoptions/
---
## AccessCacheOptions enumeration

Veri erişimi için önbellekleme seçenekleri. Birden fazla seçenek "&#x7C;" operatörü kullanılarak birleştirilebilir.

```csharp
[Flags]
public enum AccessCacheOptions
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Herhangi bir veri erişimi için önbellek yok. |
| All | `FFFFFFFFFFFFFFFF` | Çalışma kitabındaki tüm veri erişimi türleri için mümkün olan tüm optimizasyonları uygula. Optimize edilmiş erişim sırasında tüm ayarlar ve veriler değiştirilmemelidir. |
| PositionAndSize | `3` | Nesnenin (örneğin Shape) konum ve boyutunu alırken mümkün olan optimizasyonu uygulayın. Satır yüksekliği ve sütun genişliği ayarları, optimize edilmiş erişim sırasında değiştirilmemelidir. |
| CellsData | `9` | Hücre değerlerini alırken mümkün olan optimizasyonu uygulayın. Hücre verileri (Hücre ve Satır'ın veri ve ayarları) optimize edilmiş erişim sırasında değiştirilmemeli, ayrıca yeni Cell/Row nesneleri (örneğin [`Item`](../cells/item/) ile) oluşturulmamalıdır. |
| CellDisplay | `100086` | Hücrelerin görüntüleme ile ilgili sonuçlarını alırken mümkün olan optimizasyonu uygulayın ([`DisplayStringValue`](../cell/displaystringvalue/), [`GetStyle`](../cell/getstyle/), [`GetDisplayStyle`](../cell/getdisplaystyle/) vb.). Hücre verileri ve stil ile ilgili nesneler (Cell/Row/Column stilleri, sütun genişliği vb.) optimize edilmiş erişim sırasında değiştirilmemelidir. |
| GetFormula | `200000` | Formülleri alırken mümkün olan optimizasyonu uygulayın. Formül ifadesini etkileyebilecek tüm veri ve ayarlar (Çalışma sayfasının adı, Adın metni, tablonun sütunu vb.) optimize edilmiş erişim sırasında değiştirilmemelidir. |
| SetFormula | `400000` | Formülleri ayarlarken mümkün olan optimizasyonu uygulayın. Formül ifadesini etkileyebilecek tüm veri ve ayarlar (Çalışma sayfasının adı, Adın metni, tablonun sütunu vb.) optimize edilmiş erişim sırasında değiştirilmemelidir. |
| CalculateFormula | `800009` | Formülleri hesaplarken mümkün olan optimizasyonu uygulayın. Hücre verileri optimize edilmiş erişim sırasında değiştirilmemeli, ayrıca yeni nesneler (Cell, Row vb.) (örneğin [`Item`](../cells/item/) ile) oluşturulmamalıdır. |
| ConditionalFormatting | `1000009` | Koşullu biçimlendirmelerin biçimlendirme sonucunu alırken mümkün olan optimizasyonu uygulayın. Koşullu biçimlendirme sonucunu etkileyebilecek tüm veri ve ayarlar (koşullu biçimlendirme ayarları, bağımlı hücre değerleri vb.) optimize edilmiş erişim sırasında değiştirilmemelidir. |
| Validation | `2000009` | Doğrulama sonucunu alırken mümkün olan optimizasyonu uygulayın. Doğrulama sonucunu etkileyebilecek tüm veri ve ayarlar (doğrulama ayarları, bağımlı hücre değerleri vb.) optimize edilmiş erişim sırasında değiştirilmemelidir. |

### Açıklamalar

Bazı özellikler için büyük veri kümesine erişmek, arama, hesaplama gibi çok sayıda tekrarlayan ve karmaşık işlemler gerektirir ve bu işlemler ek zaman alır. Yaygın durumlarda, tüm bağımlı veriler erişim sırasında değişmez, bu yüzden bazı önbellekler oluşturularak erişim performansı artırılabilir. Bu amaçla, kullanıcıların hangi veri erişiminin olası önbellekleme mekanizmasıyla optimize edilmesi gerektiğini belirtebilmeleri için bu API'yi sağlıyoruz. Lütfen farklı seçenekler için farklı veri setlerinin "salt okunur" olması gerekebileceğini unutmayın. Ayrıca veri erişim performansı birçok faktöre bağlıdır; önbellekleme mekanizmasının kullanılması performansın artacağını garanti etmez. Bazı durumlarda, örneğin erişilecek veri kümesi küçükse, önbellek kullanmak ek zaman gerektirdiği için daha uzun sürebilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AccessCacheOptionsDemo
    {
        public static void AccessCacheOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Belirli seçeneklerle erişim önbelleğini başlat
            workbook.StartAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Önbellekten yararlanan bazı işlemleri gerçekleştir
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i + j);
                }
            }

            // Erişim önbelleğini kapat
            workbook.CloseAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Çalışma kitabını kaydedin
            workbook.Save("AccessCacheOptionsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


