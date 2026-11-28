---
title: "Enum LoadDataFilterOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LoadDataFilterOptions enum. Şablondan çalışma kitabı yüklenirken veriyi filtreleme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/loaddatafilteroptions/
---
## LoadDataFilterOptions enumeration

Şablondan çalışma kitabı yüklenirken verileri filtreleme seçeneklerini temsil eder.

```csharp
public enum LoadDataFilterOptions
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Sayfa verisi için hiçbir şey yükleme |
| All | `2147483647` | Hepsini yükle |
| CellBlank | `1` | Değeri boş olan hücreleri yükle |
| CellString | `2` | Değeri metin olan hücreleri yükle |
| CellNumeric | `4` | Değeri sayısal (tarih/saat dahil) olan hücreleri yükle |
| CellError | `8` | Hata değerine sahip hücreleri yükle |
| CellBool | `16` | Bool değerine sahip hücreleri yükle |
| CellValue | `31` | Yalnızca hücre değerlerini (tüm değer türleri) yükle |
| Formula | `32` | Hücre formüllerini yükle. |
| CellData | `67108927` | Değerleri, formülleri ve biçimlendirmeyi içeren hücre verilerini yükle |
| Chart | `256` | Grafikleri yükle |
| Shape | `402653696` | Şekilleri yükle |
| Drawing | `402653952` | Çizim nesneleri (Grafik, Resim, OleObject ve diğer tüm çizim nesneleri dahil) |
| MergedArea | `1024` | Birleştirilmiş hücreleri yükle |
| ConditionalFormatting | `2048` | Koşullu biçimlendirmeyi yükle |
| DataValidation | `4096` | Veri doğrulamalarını yükle |
| PivotTable | `8192` | Özet tabloları yükle |
| Table | `16384` | Tabloları yükle |
| Hyperlinks | `32768` | Köprüleri yükle |
| SheetSettings | `65536` | Çalışma sayfası ayarlarını yükle |
| SheetData | `403701759` | Çalışma sayfasının tüm verilerini, örneğin hücre verileri, ayarlar, nesneler, ... vb. yükle |
| BookSettings | `1048576` | Çalışma kitabı ayarlarını yükle |
| Settings | `1114112` | Çalışma kitabı ve çalışma sayfası ayarlarını yükle |
| XmlMap | `2097152` | XmlMap'i yükle |
| Structure | `4194304` | Çalışma kitabının yapısını yükle |
| DocumentProperties | `8388608` | Belge özelliklerini yükle |
| DefinedNames | `16777216` | Tanımlı Ad nesnelerini yükle |
| VBA | `33554432` | VBA projelerini yükle |
| Style | `67108864` | Hücre biçimlendirme stillerini yükle |
| Picture | `134217728` | Resimleri yükle |
| OleObject | `268435456` | OleObject'leri Yükle |
| Revision | `536870912` | Revizyon günlüklerini Yükle |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadDataFilterOptionsDemo
    {
        public static void LoadDataFilterOptionsExample()
        {
            // Yeni bir LoadOptions örneği oluştur
            LoadOptions loadOptions = new LoadOptions();

            // Özel bir LoadFilter uygulaması oluştur
            loadOptions.LoadFilter = new CustomLoadFilter();

            // Belirtilen yükleme seçenekleriyle çalışma kitabını yükle
            Workbook workbook = new Workbook("LoadDataFilterOptionsExample_original.xlsx", loadOptions);

            // Yüklenen verileri doğrulamak için çalışma kitabını kaydet
            workbook.Save("LoadDataFilterOptionsExample.xlsx");
        }

        // Özel LoadFilter uygulaması
        private class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                // Sayfa adına göre farklı filtre seçeneklerini uygula
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


