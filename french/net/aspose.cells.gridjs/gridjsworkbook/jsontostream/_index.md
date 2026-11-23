---
title: "GridJsWorkbook.JsonToStream"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridJsWorkbook method. Génère du JSON à partir du classeur en mémoire et l'écrit dans le flux spécifié. Met éventuellement en cache le JSON généré pour une récupération ultérieure plus rapide. Principales différences avec JsonToStreamByUid : cette méthode utilise l'état actuel du classeur en mémoire (champ wb). JsonToStreamByUid recharge le classeur à partir des fichiers de cache .cells sur le disque. Utilisez cette méthode lorsque vous souhaitez exporter l'état actuel du classeur après des modifications. Utilisez JsonToStreamByUid lorsque vous devez régénérer le JSON à partir d'un état de fichier précédemment mis en cache. Comportement de mise en cache lorsqu'un uid est fourni : vérifie le cache JSON avant de générer (L1 mémoire, L2 disque). En cas d'absence de cache, génère le JSON à partir du classeur en mémoire. Stocke le JSON généré dans le cache pour les requêtes futures."
type: docs
url: /fr/net/aspose.cells.gridjs/gridjsworkbook/jsontostream/
---
## GridJsWorkbook.JsonToStream method

Génère le JSON à partir du classeur en mémoire et l'écrit dans le flux spécifié. Met éventuellement en cache le JSON généré pour une récupération ultérieure plus rapide. Principales différences avec JsonToStreamByUid : - Cette méthode utilise l'état actuel du classeur en mémoire (champ wb) - JsonToStreamByUid recharge le classeur à partir des fichiers de cache .cells sur le disque - Utilisez cette méthode lorsque vous souhaitez exporter l'état actuel du classeur après des modifications - Utilisez JsonToStreamByUid lorsque vous devez régénérer le JSON à partir d'un état de fichier précédemment mis en cache. Comportement de mise en cache (lorsqu'un uid est fourni) : - Vérifie le cache JSON avant de générer (mémoire L1 + disque L2) - En cas d'absence de cache, génère le JSON à partir du classeur en mémoire - Stocke le JSON généré dans le cache pour les requêtes futures

```csharp
public void JsonToStream(Stream stream, string filename, string uid = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux de sortie où écrire les données JSON |
| nom de fichier | String | Spécifie le nom du fichier dans le JSON. Si défini sur null, le nom de fichier par défaut est : book1. |
| uid | String | Identifiant unique optionnel pour la mise en cache du JSON. Lorsqu'il est fourni, il active la recherche et le stockage dans le cache. |

### Voir aussi

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


