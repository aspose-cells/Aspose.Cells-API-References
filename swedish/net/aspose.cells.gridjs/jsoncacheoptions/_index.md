---
title: "Klass JsonCacheOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridJs.JsonCacheOptions‑klass. Konfigurationsalternativ för JSON‑cachning i GridJs. Styr både minne L1‑ och disk L2‑cachebeteende."
type: docs
url: /sv/net/aspose.cells.gridjs/jsoncacheoptions/
---
## JsonCacheOptions class

Konfigurationsalternativ för JSON-cachning i GridJs. Styr både minnes‑ (L1) och disk‑ (L2) cachebeteende.

```csharp
public class JsonCacheOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [JsonCacheOptions](jsoncacheoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CompressDisk](../../aspose.cells.gridjs/jsoncacheoptions/compressdisk/) { get; set; } | Hämtar/Anger om diskcachen ska komprimeras med Gzip (standard: true). Träder i kraft när Enable = true och standardcachen används. |
| [DiskPath](../../aspose.cells.gridjs/jsoncacheoptions/diskpath/) { get; set; } | Hämtar/Anger sökvägen till diskcache‑katalogen. Träder i kraft när Enable = true och standardcachen används. Standard: [FileCacheDirectory]/json_cache |
| [DiskTtl](../../aspose.cells.gridjs/jsoncacheoptions/diskttl/) { get; set; } | Hämtar/Anger TTL för diskcachen (standard: 24 timmar). Träder i kraft när Enable = true och standardcachen används. |
| [Enable](../../aspose.cells.gridjs/jsoncacheoptions/enable/) { get; set; } | Hämtar/Anger om JSON‑cachning ska aktiveras för snabbare svar. När den är aktiverad kommer GridJs att cacha den genererade JSON‑en och återanvända den för efterföljande begäranden. Standardvärdet är false. Obs: Du måste ange Implementation för att använda anpassad cache‑lagring. |
| [EnableDisk](../../aspose.cells.gridjs/jsoncacheoptions/enabledisk/) { get; set; } | Hämtar/Anger om diskcachen ska aktiveras (standard: true). Träder i kraft när Enable = true och standardcachen används. |
| [Implementation](../../aspose.cells.gridjs/jsoncacheoptions/implementation/) { get; set; } | Hämtar/Anger den anpassade JSON‑cache‑implementationen. Om den inte anges kommer GridJs att använda standard‑minne + disk‑cache. |
| [MaxDiskSizeMB](../../aspose.cells.gridjs/jsoncacheoptions/maxdisksizemb/) { get; set; } | Hämtar/Anger maximal storlek för diskcachen i MB (standard: 500 MB). Träder i kraft när Enable = true och standardcachen används. |
| [MaxMemoryEntries](../../aspose.cells.gridjs/jsoncacheoptions/maxmemoryentries/) { get; set; } | Hämtar/Anger maximalt antal poster i minnescachen (standard: 1000). Träder i kraft när Enable = true och standardcachen används. |
| [MemoryTtl](../../aspose.cells.gridjs/jsoncacheoptions/memoryttl/) { get; set; } | Hämtar/Anger TTL för minnescachen (standard: 1 timme). Träder i kraft när Enable = true och standardcachen används. |

### Se även

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


