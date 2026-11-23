---
title: "类 JsonCacheOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridJs.JsonCacheOptions 类。GridJs 中 JSON 缓存的配置选项。控制内存 L1 和磁盘 L2 缓存行为"
type: docs
url: /zh/net/aspose.cells.gridjs/jsoncacheoptions/
---
## JsonCacheOptions class

GridJs 中 JSON 缓存的配置选项。控制内存 (L1) 和磁盘 (L2) 缓存行为。

```csharp
public class JsonCacheOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [JsonCacheOptions](jsoncacheoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CompressDisk](../../aspose.cells.gridjs/jsoncacheoptions/compressdisk/) { get; set; } | 获取/设置 是否使用 Gzip 压缩磁盘缓存（默认：true）。当 Enable = true 且使用默认缓存时生效。 |
| [DiskPath](../../aspose.cells.gridjs/jsoncacheoptions/diskpath/) { get; set; } | 获取/设置 磁盘缓存目录路径。当 Enable = true 且使用默认缓存时生效。默认值: [FileCacheDirectory]/json_cache |
| [DiskTtl](../../aspose.cells.gridjs/jsoncacheoptions/diskttl/) { get; set; } | 获取/设置 磁盘缓存的 TTL（默认：24 小时）。当 Enable = true 且使用默认缓存时生效。 |
| [Enable](../../aspose.cells.gridjs/jsoncacheoptions/enable/) { get; set; } | 获取/设置 是否启用 JSON 缓存以获得更快的响应。启用后，GridJs 将缓存生成的 JSON 并在后续请求中复用。默认值为 false。注意：需要设置 Implementation 以使用自定义缓存存储。 |
| [EnableDisk](../../aspose.cells.gridjs/jsoncacheoptions/enabledisk/) { get; set; } | 获取/设置 是否启用磁盘缓存（默认：true）。当 Enable = true 且使用默认缓存时生效。 |
| [Implementation](../../aspose.cells.gridjs/jsoncacheoptions/implementation/) { get; set; } | 获取/设置 自定义 JSON 缓存实现。如果未设置，GridJs 将使用默认的内存 + 磁盘缓存。 |
| [MaxDiskSizeMB](../../aspose.cells.gridjs/jsoncacheoptions/maxdisksizemb/) { get; set; } | 获取/设置 最大磁盘缓存大小（单位 MB，默认：500 MB）。当 Enable = true 且使用默认缓存时生效。 |
| [MaxMemoryEntries](../../aspose.cells.gridjs/jsoncacheoptions/maxmemoryentries/) { get; set; } | 获取/设置 内存缓存的最大条目数（默认：1000）。当 Enable = true 且使用默认缓存时生效。 |
| [MemoryTtl](../../aspose.cells.gridjs/jsoncacheoptions/memoryttl/) { get; set; } | 获取/设置 内存缓存的 TTL（默认：1 小时）。当 Enable = true 且使用默认缓存时生效。 |

### 另请参见

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


