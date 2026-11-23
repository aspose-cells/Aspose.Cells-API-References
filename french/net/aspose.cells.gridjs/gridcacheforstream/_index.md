---
title: "Classe GridCacheForStream"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridJs.GridCacheForStream. Cette classe contient les opérations de cache pour GridJs. L'utilisateur doit implémenter sa propre logique métier de stockage basée sur celle-ci"
type: docs
url: /fr/net/aspose.cells.gridjs/gridcacheforstream/
---
## GridCacheForStream class

Cette classe contient les opérations de cache pour GridJs. L'utilisateur doit implémenter sa propre logique métier pour le stockage basée sur celle-ci..

```csharp
public abstract class GridCacheForStream
```

## Méthodes

| Nom | Description |
| --- | --- |
| abstract [GetFileUrl](../../aspose.cells.gridjs/gridcacheforstream/getfileurl/)(string) | Implémentez cette méthode pour obtenir l'URL du fichier depuis le cache. |
| abstract [IsExisted](../../aspose.cells.gridjs/gridcacheforstream/isexisted/)(string) | Vérifie si le cache avec l'uid existe |
| abstract [LoadStream](../../aspose.cells.gridjs/gridcacheforstream/loadstream/)(string) | Implémentez cette méthode pour charger le cache avec la clé uid et renvoyer le flux depuis le cache. |
| abstract [SaveStream](../../aspose.cells.gridjs/gridcacheforstream/savestream/)(Stream, string) | Implémentez cette méthode pour enregistrer le cache, en sauvegardant le flux dans le cache avec la clé uid. |

### Voir aussi

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


