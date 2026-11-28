---
title: "Sınıf JsonCacheOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridJs.JsonCacheOptions sınıfı. GridJs'te JSON önbellekleme için yapılandırma seçenekleri. Hem bellek L1 hem de disk L2 önbellek davranışını kontrol eder."
type: docs
url: /tr/net/aspose.cells.gridjs/jsoncacheoptions/
---
## JsonCacheOptions class

GridJs'te JSON önbellekleme için yapılandırma seçenekleri. Bellek (L1) ve disk (L2) önbellek davranışını kontrol eder.

```csharp
public class JsonCacheOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [JsonCacheOptions](jsoncacheoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CompressDisk](../../aspose.cells.gridjs/jsoncacheoptions/compressdisk/) { get; set; } | Alır/Ayarlar Gzip kullanarak disk önbelleğini sıkıştırıp sıkıştırmayacağını (varsayılan: true). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur. |
| [DiskPath](../../aspose.cells.gridjs/jsoncacheoptions/diskpath/) { get; set; } | Alır/Ayarlar disk önbelleği dizini yolunu. Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur. Varsayılan: [FileCacheDirectory]/json_cache |
| [DiskTtl](../../aspose.cells.gridjs/jsoncacheoptions/diskttl/) { get; set; } | Alır/Ayarlar disk önbelleği için TTL'yi (varsayılan: 24 saat). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur. |
| [Enable](../../aspose.cells.gridjs/jsoncacheoptions/enable/) { get; set; } | Alır/Ayarlar JSON önbelleklemesini daha hızlı yanıt için etkinleştirip etkinleştirmeyeceğini. Etkinleştirildiğinde, GridJs oluşturulan JSON'ı önbelleğe alır ve sonraki isteklerde yeniden kullanır. Varsayılan değer false'tur. Not: Özel önbellek depolama kullanmak için Implementation'ı ayarlamanız gerekir. |
| [EnableDisk](../../aspose.cells.gridjs/jsoncacheoptions/enabledisk/) { get; set; } | Alır/Ayarlar disk önbelleğini etkinleştirip etkinleştirmeyeceğini (varsayılan: true). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur. |
| [Implementation](../../aspose.cells.gridjs/jsoncacheoptions/implementation/) { get; set; } | Alır/Ayarlar özel JSON önbellek uygulamasını. Ayarlanmamışsa, GridJs varsayılan bellek + disk önbelleğini kullanır. |
| [MaxDiskSizeMB](../../aspose.cells.gridjs/jsoncacheoptions/maxdisksizemb/) { get; set; } | Alır/Ayarlar maksimum disk önbellek boyutunu MB cinsinden (varsayılan: 500 MB). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur. |
| [MaxMemoryEntries](../../aspose.cells.gridjs/jsoncacheoptions/maxmemoryentries/) { get; set; } | Alır/Ayarlar bellek önbelleğinde maksimum giriş sayısını (varsayılan: 1000). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur. |
| [MemoryTtl](../../aspose.cells.gridjs/jsoncacheoptions/memoryttl/) { get; set; } | Alır/Ayarlar bellek önbelleği için TTL'yi (varsayılan: 1 saat). Enable = true olduğunda ve varsayılan önbellek kullanıldığında etkili olur. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


