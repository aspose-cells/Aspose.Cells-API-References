---
title: "Класс JsonCacheOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridJs.JsonCacheOptions. Параметры конфигурации кэширования JSON в GridJs. Управляет поведением кэша в памяти L1 и на диске L2."
type: docs
url: /ru/net/aspose.cells.gridjs/jsoncacheoptions/
---
## JsonCacheOptions class

Параметры конфигурации кэширования JSON в GridJs. Управляет поведением кэша в памяти (L1) и на диске (L2).

```csharp
public class JsonCacheOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [JsonCacheOptions](jsoncacheoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CompressDisk](../../aspose.cells.gridjs/jsoncacheoptions/compressdisk/) { get; set; } | Получает/Устанавливает, следует ли сжимать кэш диска с помощью Gzip (по умолчанию: true). Влияет, когда Enable = true и используется кэш по умолчанию. |
| [DiskPath](../../aspose.cells.gridjs/jsoncacheoptions/diskpath/) { get; set; } | Получает/Устанавливает путь к каталогу кэша диска. Влияет, когда Enable = true и используется кэш по умолчанию. По умолчанию: [FileCacheDirectory]/json_cache |
| [DiskTtl](../../aspose.cells.gridjs/jsoncacheoptions/diskttl/) { get; set; } | Получает/Устанавливает TTL для кэша диска (по умолчанию: 24 часа). Влияет, когда Enable = true и используется кэш по умолчанию. |
| [Enable](../../aspose.cells.gridjs/jsoncacheoptions/enable/) { get; set; } | Получает/Устанавливает, следует ли включить кэширование JSON для более быстрого отклика. При включении GridJs будет кэшировать сгенерированный JSON и повторно использовать его для последующих запросов. Значение по умолчанию — false. Примечание: необходимо установить Implementation для использования пользовательского хранилища кэша. |
| [EnableDisk](../../aspose.cells.gridjs/jsoncacheoptions/enabledisk/) { get; set; } | Получает/Устанавливает, следует ли включить кэш диска (по умолчанию: true). Влияет, когда Enable = true и используется кэш по умолчанию. |
| [Implementation](../../aspose.cells.gridjs/jsoncacheoptions/implementation/) { get; set; } | Получает/Устанавливает пользовательскую реализацию кэша JSON. Если не задано, GridJs будет использовать кэш памяти + диска по умолчанию. |
| [MaxDiskSizeMB](../../aspose.cells.gridjs/jsoncacheoptions/maxdisksizemb/) { get; set; } | Получает/Устанавливает максимальный размер кэша диска в МБ (по умолчанию: 500 МБ). Влияет, когда Enable = true и используется кэш по умолчанию. |
| [MaxMemoryEntries](../../aspose.cells.gridjs/jsoncacheoptions/maxmemoryentries/) { get; set; } | Получает/Устанавливает максимальное количество записей в кэше памяти (по умолчанию: 1000). Влияет, когда Enable = true и используется кэш по умолчанию. |
| [MemoryTtl](../../aspose.cells.gridjs/jsoncacheoptions/memoryttl/) { get; set; } | Получает/Устанавливает TTL для кэша памяти (по умолчанию: 1 час). Влияет, когда Enable = true и используется кэш по умолчанию. |

### См. также

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


