---
title: "Klasse JsonCacheOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridJs.JsonCacheOptions Klasse. Konfigurationsoptionen für das JSON-Caching in GridJs. Steuert das Verhalten des Speicher‑L1‑ und Festplatten‑L2‑Cache."
type: docs
url: /de/net/aspose.cells.gridjs/jsoncacheoptions/
---
## JsonCacheOptions class

Konfigurationsoptionen für das JSON‑Caching in GridJs. Steuert das Verhalten des Speicher‑ (L1) und Festplatten‑ (L2) Caches.

```csharp
public class JsonCacheOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [JsonCacheOptions](jsoncacheoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CompressDisk](../../aspose.cells.gridjs/jsoncacheoptions/compressdisk/) { get; set; } | Liest/Setzt, ob der Festplatten-Cache mit Gzip komprimiert wird (Standard: true). Wird wirksam, wenn Enable = true und der Standard‑Cache verwendet wird. |
| [DiskPath](../../aspose.cells.gridjs/jsoncacheoptions/diskpath/) { get; set; } | Liest/Setzt den Pfad des Festplatten‑Cache‑Verzeichnisses. Wird wirksam, wenn Enable = true und der Standard‑Cache verwendet wird. Standard: [FileCacheDirectory]/json_cache |
| [DiskTtl](../../aspose.cells.gridjs/jsoncacheoptions/diskttl/) { get; set; } | Liest/Setzt die TTL für den Festplatten‑Cache (Standard: 24 Stunden). Wird wirksam, wenn Enable = true und der Standard‑Cache verwendet wird. |
| [Enable](../../aspose.cells.gridjs/jsoncacheoptions/enable/) { get; set; } | Liest/Setzt, ob JSON-Caching für schnellere Antworten aktiviert wird. Wenn aktiviert, cached GridJs das erzeugte JSON und verwendet es für nachfolgende Anfragen erneut. Der Standardwert ist false. Hinweis: Sie müssen Implementation setzen, um benutzerdefinierten Cache‑Speicher zu verwenden. |
| [EnableDisk](../../aspose.cells.gridjs/jsoncacheoptions/enabledisk/) { get; set; } | Liest/Setzt, ob der Festplatten‑Cache aktiviert wird (Standard: true). Wird wirksam, wenn Enable = true und der Standard‑Cache verwendet wird. |
| [Implementation](../../aspose.cells.gridjs/jsoncacheoptions/implementation/) { get; set; } | Liest/Setzt die benutzerdefinierte JSON‑Cache‑Implementierung. Wenn nicht gesetzt, verwendet GridJs den Standard‑Speicher‑+‑Festplatten‑Cache. |
| [MaxDiskSizeMB](../../aspose.cells.gridjs/jsoncacheoptions/maxdisksizemb/) { get; set; } | Liest/Setzt die maximale Größe des Festplatten‑Cache in MB (Standard: 500 MB). Wird wirksam, wenn Enable = true und der Standard‑Cache verwendet wird. |
| [MaxMemoryEntries](../../aspose.cells.gridjs/jsoncacheoptions/maxmemoryentries/) { get; set; } | Liest/Setzt die maximale Anzahl von Einträgen im Speicher‑Cache (Standard: 1000). Wird wirksam, wenn Enable = true und der Standard‑Cache verwendet wird. |
| [MemoryTtl](../../aspose.cells.gridjs/jsoncacheoptions/memoryttl/) { get; set; } | Liest/Setzt die TTL für den Speicher‑Cache (Standard: 1 Stunde). Wird wirksam, wenn Enable = true und der Standard‑Cache verwendet wird. |

### Siehe auch

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


