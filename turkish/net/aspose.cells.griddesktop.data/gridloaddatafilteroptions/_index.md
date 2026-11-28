---
title: "Enum GridLoadDataFilterOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridDesktop.Data.GridLoadDataFilterOptions enum. Şablondan çalışma kitabı yüklenirken verileri filtreleme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridloaddatafilteroptions/
---
## GridLoadDataFilterOptions enumeration

Şablondan çalışma kitabı yüklenirken verileri filtreleme seçeneklerini temsil eder.

```csharp
public enum GridLoadDataFilterOptions
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


