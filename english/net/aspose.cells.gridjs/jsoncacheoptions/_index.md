---
title: Class JsonCacheOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.GridJs.JsonCacheOptions class. Configuration options for JSON caching in GridJs. Controls both memory L1 and disk L2 cache behavior
type: docs
url: /net/aspose.cells.gridjs/jsoncacheoptions/
---
## JsonCacheOptions class

Configuration options for JSON caching in GridJs. Controls both memory (L1) and disk (L2) cache behavior.

```csharp
public class JsonCacheOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [JsonCacheOptions](jsoncacheoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [CompressDisk](../../aspose.cells.gridjs/jsoncacheoptions/compressdisk/) { get; set; } | Gets/Sets whether to compress disk cache using Gzip (default: true). Takes effect when Enable = true and using default cache. |
| [DiskPath](../../aspose.cells.gridjs/jsoncacheoptions/diskpath/) { get; set; } | Gets/Sets the disk cache directory path. Takes effect when Enable = true and using default cache. Default: [FileCacheDirectory]/json_cache |
| [DiskTtl](../../aspose.cells.gridjs/jsoncacheoptions/diskttl/) { get; set; } | Gets/Sets the TTL for disk cache (default: 24 hours). Takes effect when Enable = true and using default cache. |
| [Enable](../../aspose.cells.gridjs/jsoncacheoptions/enable/) { get; set; } | Gets/Sets whether to enable JSON caching for faster response. When enabled, GridJs will cache the generated JSON and reuse it for subsequent requests. The default value is false. Note: You need to set Implementation to use custom cache storage. |
| [EnableDisk](../../aspose.cells.gridjs/jsoncacheoptions/enabledisk/) { get; set; } | Gets/Sets whether to enable disk cache (default: true). Takes effect when Enable = true and using default cache. |
| [Implementation](../../aspose.cells.gridjs/jsoncacheoptions/implementation/) { get; set; } | Gets/Sets the custom JSON cache implementation. If not set, GridJs will use the default memory + disk cache. |
| [MaxDiskSizeMB](../../aspose.cells.gridjs/jsoncacheoptions/maxdisksizemb/) { get; set; } | Gets/Sets the maximum disk cache size in MB (default: 500 MB). Takes effect when Enable = true and using default cache. |
| [MaxMemoryEntries](../../aspose.cells.gridjs/jsoncacheoptions/maxmemoryentries/) { get; set; } | Gets/Sets the maximum number of entries in memory cache (default: 1000). Takes effect when Enable = true and using default cache. |
| [MemoryTtl](../../aspose.cells.gridjs/jsoncacheoptions/memoryttl/) { get; set; } | Gets/Sets the TTL for memory cache (default: 1 hour). Takes effect when Enable = true and using default cache. |

### See Also

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


