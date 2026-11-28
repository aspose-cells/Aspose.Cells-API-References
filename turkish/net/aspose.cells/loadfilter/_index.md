---
title: "Sınıf LoadFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LoadFilter sınıfı. Şablondan çalışma kitabı yüklenirken veri yükleme seçenekleri sağlayan filtreyi temsil eder"
type: docs
url: /tr/net/aspose.cells/loadfilter/
---
## LoadFilter class

Şablondan çalışma kitabı yüklenirken veri yükleme seçeneklerini sağlayan filtreyi temsil eder.

```csharp
public class LoadFilter
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LoadFilter](loadfilter/#constructor)() | Varsayılan filtre seçenekleri LoadDataFilterOptions.All ile bir LoadFilter oluşturur. |
| [LoadFilter](loadfilter/#constructor_1)(LoadDataFilterOptions) | Verilen filtre seçenekleriyle bir LoadFilter oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions/) { get; set; } | Yüklenmesi gereken veriyi belirtmek için filtre seçenekleri. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder/) { get; } | Yüklenmesi gereken sayfaları (indekslerini) ve sıralamayı belirtir. Varsayılan değer null'dır ve bu, şablon dosyasındaki tüm sayfaların varsayılan sırayla yüklenmesini ifade eder. Null değilse ve bazı sayfa indeksleri döndürülen dizide yoksa, o sayfa yüklenmez. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet/)(Worksheet) | Belirtilen çalışma sayfası yüklenmeden önce filtre seçeneklerini hazırlar. Kullanıcının LoadFilter uygulaması burada LoadDataFilterOptions'ı değiştirerek bu çalışma sayfası için verinin nasıl yükleneceğini belirtebilir. |

### Açıklamalar

Kullanıcı filtre seçeneklerini belirtebilir veya verinin nasıl yükleneceğini belirtmek için kendi LoadFilter'ını uygulayabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterDemo
    {
        public static void LoadFilterExample()
        {
            // LoadOptions oluşturun ve LoadFilter'ı ayarlayın
            LoadOptions opts = new LoadOptions();
            opts.LoadFilter = new CustomLoadFilter();

            // Belirtilen LoadOptions ile çalışma kitabını yükleyin
            Workbook wb = new Workbook("LoadFilterExample_original.xlsx", opts);

            // LoadFilter etkisini görmek için çalışma kitabını kaydedin
            wb.Save("LoadFilterExample.xlsx");
        }

        // Özel LoadFilter uygulaması
        public class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                if (sheet.Name == "Sheet1")
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.All;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


