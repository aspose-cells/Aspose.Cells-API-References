---
title: LoadFilter
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma kitabını şablondan yüklerken veri yükleme seçenekleri sağlayan filtreyi temsil eder.
type: docs
weight: 3980
url: /tr/net/aspose.cells/loadfilter/
---
## LoadFilter class

Çalışma kitabını şablondan yüklerken veri yükleme seçenekleri sağlayan filtreyi temsil eder.

```csharp
public class LoadFilter
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [LoadFilter](loadfilter#constructor)() | Varsayılan filtre seçenekleriyle bir LoadFilter oluşturur LoadDataFilterOptions.All. |
| [LoadFilter](loadfilter#constructor_1)(LoadDataFilterOptions) | Verilen filtre seçenekleriyle bir LoadFilter oluşturur. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions) { get; set; } | Hangi verilerin yüklenmesi gerektiğini belirtmek için filtre seçenekleri. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder) { get; } | Yüklenecek sayfaları (endeksleri) ve sırayı belirtir. Varsayılan boştur, bu, şablon dosyasındaki tüm sayfaların varsayılan sırayla yüklenmesini belirtir. Boş değilse ve bazı sayfanın dizini döndürülen dizide değilse, sayfa yüklenmeyecek. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet)(Worksheet) | Verilen çalışma sayfasını yüklemeden önce filtre seçeneklerini hazırlar. Kullanıcının LoadFilter uygulaması, bu çalışma sayfası için verilerin nasıl yükleneceğini belirtmek için buradaki LoadDataFilterOptions'ı değiştirebilir. |

### Notlar

Kullanıcı, verilerin nasıl yükleneceğini belirtmek için filtre seçeneklerini belirleyebilir veya kendi LoadFilter'ını uygulayabilir.

### Örnekler

Aşağıdaki örnek, çalışma sayfasının özelliklerine göre filtre seçeneklerinin nasıl belirleneceğini gösterir.

```csharp
[C#]
Workbook wb = new Workbook(template, new LoadOptions() { LoadFilter = new LoadFilterSheet() });
//Özel LoadFilter uygulaması
class LoadFilterSheet : LoadFilter
{
    public override void StartSheet(Worksheet sheet) 
    {
        if (sheet.Name == "Sheet1")
        {
            LoadDataFilterOptions = Aspose.Cells.LoadDataFilterOptions.All;
        }
        else
        {
            LoadDataFilterOptions = Aspose.Cells.LoadDataFilterOptions.None;
        }
    }
}
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->