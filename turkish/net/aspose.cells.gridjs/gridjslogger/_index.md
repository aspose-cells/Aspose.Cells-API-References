---
title: "Sınıf GridJsLogger"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridJs.GridJsLogger sınıfı. GridJs sunucusu için hafif bir günlükleme sistemi sağlar. Yapılandırılabilir günlük seviyeleriyle konsol ve dosya çıktısını destekler. Varsayılan seviye None'dur. DEBUG derlemesinde varsayılan seviye Debug'tir ve tüm mesajları çıktılar. Günlük dosyası döndürmeyi gün/hafta/ay bazında destekler."
type: docs
url: /tr/net/aspose.cells.gridjs/gridjslogger/
---
## GridJsLogger class

GridJs sunucusu için hafif bir günlükleme sistemi sağlar. Yapılandırılabilir günlük seviyeleriyle konsol ve dosya çıktısını destekler. Varsayılan seviye Yok'tur. DEBUG derlemesinde, varsayılan seviye Debug'tir (tüm mesajları çıktılar). Gün, hafta veya ay bazında günlük dosyası döndürmeyi destekler.

```csharp
public static class GridJsLogger
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| static [EnableConsoleOutput](../../aspose.cells.gridjs/gridjslogger/enableconsoleoutput/) { get; set; } | Günlük mesajlarını konsola çıkartıp çıkarmayacağını alır veya ayarlar. Varsayılan değer false'tur. |
| static [EnableFileOutput](../../aspose.cells.gridjs/gridjslogger/enablefileoutput/) { get; set; } | Günlük mesajlarını bir dosyaya çıkartıp çıkarmayacağını alır veya ayarlar. Varsayılan değer false'tur. Etkinleştirmeden önce [`SetLogFile`](./setlogfile/) veya [`SetLogDirectory`](./setlogdirectory/) çağrılmalıdır. |
| static [Level](../../aspose.cells.gridjs/gridjslogger/level/) { get; set; } | Minimum günlük seviyesini alır veya ayarlar. Bu seviyenin altındaki mesajlar yok sayılır. Varsayılan değer None'dur. |
| static [LogFilePath](../../aspose.cells.gridjs/gridjslogger/logfilepath/) { get; } | Mevcut günlük dosyası yolunu alır; ayarlanmamışsa null döner. |
| static [MaxFileSize](../../aspose.cells.gridjs/gridjslogger/maxfilesize/) { get; set; } | Döndürmeden önce tek bir günlük dosyasının maksimum boyutunu (bayt cinsinden) alır veya ayarlar. Yalnızca döndürme etkin olduğunda geçerlidir. 0, boyut sınırlaması olmadığı anlamına gelir. Varsayılan değer 0'dır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [CloseLogFile](../../aspose.cells.gridjs/gridjslogger/closelogfile/)() | Günlük dosyası yazarını kapatır ve dosya çıktısını devre dışı bırakır. |
| static [Debug](../../aspose.cells.gridjs/gridjslogger/debug/)(string) | Bir debug seviyesinde mesaj kaydeder. |
| static [Error](../../aspose.cells.gridjs/gridjslogger/error/)(string) | Bir hata seviyesinde mesaj kaydeder. |
| static [Info](../../aspose.cells.gridjs/gridjslogger/info/)(string) | Bir bilgi seviyesinde mesaj kaydeder. |
| static [Log](../../aspose.cells.gridjs/gridjslogger/log/)(GridJsLogLevel, string) | Belirtilen seviyede bir mesaj kaydeder. |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory)(string) | Günlük dizinini günlük döndürme dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. Günlük dosyaları şu şekilde adlandırılır: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_1)(string, GridJsLogRolling) | Günlük dizinini döndürme dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. Günlük dosyaları şu şekilde adlandırılır: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_2)(string, GridJsLogRolling, string) | Günlük dizinini döndürme dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. Günlük dosyaları şu şekilde adlandırılır: {prefix}_{period}.log Örnekler: gridjs_2026-07-27.log (Günlük), gridjs_2026-W30.log (Haftalık), gridjs_2026-07.log (Aylık) |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile)(string) | Günlük dosyası yolunu ayarlar ve dosya çıktısını etkinleştirir (tek dosya modu, döndürme yok). Mevcut dosyaya ekler. |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile_1)(string, bool) | Günlük dosyası yolunu ayarlar ve dosya çıktısını etkinleştirir (tek dosya modu, döndürme yok). |
| static [Warn](../../aspose.cells.gridjs/gridjslogger/warn/)(string) | Uyarı seviyesinde bir mesaj kaydeder. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


