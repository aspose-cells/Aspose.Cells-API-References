---
title: "Classe JsonCacheOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridJs.JsonCacheOptions. Options de configuration pour le cache JSON dans GridJs. Contrôle le comportement du cache mémoire L1 et disque L2."
type: docs
url: /fr/net/aspose.cells.gridjs/jsoncacheoptions/
---
## JsonCacheOptions class

Options de configuration pour la mise en cache JSON dans GridJs. Contrôle le comportement du cache mémoire (L1) et disque (L2).

```csharp
public class JsonCacheOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [JsonCacheOptions](jsoncacheoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CompressDisk](../../aspose.cells.gridjs/jsoncacheoptions/compressdisk/) { get; set; } | Obtient/Définit si la compression du cache disque avec Gzip est activée (par défaut : true). Prend effet lorsque Enable = true et en utilisant le cache par défaut. |
| [DiskPath](../../aspose.cells.gridjs/jsoncacheoptions/diskpath/) { get; set; } | Obtient/Définit le chemin du répertoire du cache disque. Prend effet lorsque Enable = true et en utilisant le cache par défaut. Valeur par défaut : [FileCacheDirectory]/json_cache |
| [DiskTtl](../../aspose.cells.gridjs/jsoncacheoptions/diskttl/) { get; set; } | Obtient/Définit le TTL du cache disque (par défaut : 24 heures). Prend effet lorsque Enable = true et en utilisant le cache par défaut. |
| [Enable](../../aspose.cells.gridjs/jsoncacheoptions/enable/) { get; set; } | Obtient/Définit si la mise en cache JSON est activée pour une réponse plus rapide. Lorsqu'elle est activée, GridJs mettra en cache le JSON généré et le réutilisera pour les requêtes suivantes. La valeur par défaut est false. Remarque : vous devez définir Implementation pour utiliser un stockage de cache personnalisé. |
| [EnableDisk](../../aspose.cells.gridjs/jsoncacheoptions/enabledisk/) { get; set; } | Obtient/Définit si le cache disque est activé (par défaut : true). Prend effet lorsque Enable = true et en utilisant le cache par défaut. |
| [Implementation](../../aspose.cells.gridjs/jsoncacheoptions/implementation/) { get; set; } | Obtient/Définit l'implémentation personnalisée du cache JSON. Si elle n'est pas définie, GridJs utilisera le cache mémoire + disque par défaut. |
| [MaxDiskSizeMB](../../aspose.cells.gridjs/jsoncacheoptions/maxdisksizemb/) { get; set; } | Obtient/Définit la taille maximale du cache disque en Mo (par défaut : 500 Mo). Prend effet lorsque Enable = true et en utilisant le cache par défaut. |
| [MaxMemoryEntries](../../aspose.cells.gridjs/jsoncacheoptions/maxmemoryentries/) { get; set; } | Obtient/Définit le nombre maximal d'entrées dans le cache mémoire (par défaut : 1000). Prend effet lorsque Enable = true et en utilisant le cache par défaut. |
| [MemoryTtl](../../aspose.cells.gridjs/jsoncacheoptions/memoryttl/) { get; set; } | Obtient/Définit le TTL du cache mémoire (par défaut : 1 heure). Prend effet lorsque Enable = true et en utilisant le cache par défaut. |

### Voir aussi

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


