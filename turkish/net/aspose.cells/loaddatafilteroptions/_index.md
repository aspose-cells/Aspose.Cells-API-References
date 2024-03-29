---
title: LoadDataFilterOptions
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma kitabını şablondan yüklerken verileri filtreleme seçeneklerini temsil eder.
type: docs
weight: 3970
url: /tr/net/aspose.cells/loaddatafilteroptions/
---
## LoadDataFilterOptions enumeration

Çalışma kitabını şablondan yüklerken verileri filtreleme seçeneklerini temsil eder.

```csharp
public enum LoadDataFilterOptions
```

### değerler

| İsim | Değer | Tanım |
| --- | --- | --- |
| None | `0` | Sayfa verileri için hiçbir şey yükleme |
| All | `2147483647` | Tümünü yükle |
| CellBlank | `1` | Değeri boş olan hücreleri yükleyin |
| CellString | `2` | Değeri string olan hücreleri yükleyin |
| CellNumeric | `4` | Değeri sayısal olan hücreleri yükleyin(tarih saat dahil) |
| CellError | `8` | Değeri error olan hücreleri yükleyin |
| CellBool | `16` | Değeri bool olan hücreleri yükleyin |
| CellValue | `31` | Yalnızca yük hücreleri değeri (tüm değer türleri) |
| Formula | `32` | Hücre formüllerini yükleyin. |
| CellData | `67108927` | Değerler, formüller ve biçimlendirme dahil hücre verilerini yükleyin |
| Chart | `256` | Grafikleri yükle |
| Shape | `402653696` | Şekilleri yükle |
| Drawing | `402653952` | Çizim nesneleri(Grafik, Resim, OleObject ve diğer tüm çizim nesneleri dahil) |
| MergedArea | `1024` | Birleştirilmiş hücreleri yükle |
| ConditionalFormatting | `2048` | Koşullu biçimlendirmeyi yükle |
| DataValidation | `4096` | Veri doğrulamalarını yükleyin |
| PivotTable | `8192` | Özet tabloları yükleyin |
| Table | `16384` | Tabloları yükle |
| Hyperlinks | `32768` | Köprüleri yükle |
| SheetSettings | `65536` | Çalışma sayfası için ayarları yükleyin |
| SheetData | `403701759` | Hücre verileri, ayarlar, nesneler, ...etc. gibi çalışma sayfasının tüm verilerini yükleyin |
| BookSettings | `1048576` | Çalışma kitabı için ayarları yükleyin |
| Settings | `1114112` | Çalışma kitabı ve çalışma sayfası için ayarları yükleyin |
| XmlMap | `2097152` | XmlMap Yükle |
| Structure | `4194304` | Çalışma kitabının yükleme yapısı |
| DocumentProperties | `8388608` | Belge özelliklerini yükle |
| DefinedNames | `16777216` | Tanımlanmış Ad nesnelerini yükle |
| VBA | `33554432` | VBA projelerini yükleyin |
| Style | `67108864` | Hücre biçimlendirmesi için stilleri yükleyin |
| Picture | `134217728` | Resimleri yükle |
| OleObject | `268435456` | OleObjects'i Yükle |
| Revision | `536870912` | Revizyon günlüklerini yükle |

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
