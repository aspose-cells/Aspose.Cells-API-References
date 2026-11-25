---
title: "Classe JsonCacheOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridJs.JsonCacheOptions. Opzioni di configurazione per la cache JSON in GridJs. Controlla sia la cache di memoria L1 sia quella su disco L2."
type: docs
url: /it/net/aspose.cells.gridjs/jsoncacheoptions/
---
## JsonCacheOptions class

Opzioni di configurazione per la cache JSON in GridJs. Controlla il comportamento della cache sia in memoria (L1) che su disco (L2).

```csharp
public class JsonCacheOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [JsonCacheOptions](jsoncacheoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CompressDisk](../../aspose.cells.gridjs/jsoncacheoptions/compressdisk/) { get; set; } | Ottiene/Imposta se comprimere la cache su disco usando Gzip (predefinito: true). Ha effetto quando Enable = true e si utilizza la cache predefinita. |
| [DiskPath](../../aspose.cells.gridjs/jsoncacheoptions/diskpath/) { get; set; } | Ottiene/Imposta il percorso della directory della cache su disco. Ha effetto quando Enable = true e si utilizza la cache predefinita. Predefinito: [FileCacheDirectory]/json_cache |
| [DiskTtl](../../aspose.cells.gridjs/jsoncacheoptions/diskttl/) { get; set; } | Ottiene/Imposta il TTL per la cache su disco (predefinito: 24 ore). Ha effetto quando Enable = true e si utilizza la cache predefinita. |
| [Enable](../../aspose.cells.gridjs/jsoncacheoptions/enable/) { get; set; } | Ottiene/Imposta se abilitare la cache JSON per una risposta più veloce. Quando abilitato, GridJs memorizzerà nella cache il JSON generato e lo riutilizzerà per le richieste successive. Il valore predefinito è false. Nota: è necessario impostare Implementation per utilizzare un archivio cache personalizzato. |
| [EnableDisk](../../aspose.cells.gridjs/jsoncacheoptions/enabledisk/) { get; set; } | Ottiene/Imposta se abilitare la cache su disco (predefinito: true). Ha effetto quando Enable = true e si utilizza la cache predefinita. |
| [Implementation](../../aspose.cells.gridjs/jsoncacheoptions/implementation/) { get; set; } | Ottiene/Imposta l'implementazione personalizzata della cache JSON. Se non impostata, GridJs utilizzerà la cache predefinita in memoria + su disco. |
| [MaxDiskSizeMB](../../aspose.cells.gridjs/jsoncacheoptions/maxdisksizemb/) { get; set; } | Ottiene/Imposta la dimensione massima della cache su disco in MB (predefinito: 500 MB). Ha effetto quando Enable = true e si utilizza la cache predefinita. |
| [MaxMemoryEntries](../../aspose.cells.gridjs/jsoncacheoptions/maxmemoryentries/) { get; set; } | Ottiene/Imposta il numero massimo di voci nella cache in memoria (predefinito: 1000). Ha effetto quando Enable = true e si utilizza la cache predefinita. |
| [MemoryTtl](../../aspose.cells.gridjs/jsoncacheoptions/memoryttl/) { get; set; } | Ottiene/Imposta il TTL per la cache in memoria (predefinito: 1 ora). Ha effetto quando Enable = true e si utilizza la cache predefinita. |

### Vedi anche

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


