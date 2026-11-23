---
title: "Interface IGridJsJsonCache"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.GridJs.IGridJsJsonCache. Interface de cache JSON que les clients implémentent avec des stratégies de stockage et d'invalidation spécifiques"
type: docs
url: /fr/net/aspose.cells.gridjs/igridjsjsoncache/
---
## IGridJsJsonCache interface

Interface de cache JSON - les clients implémentent des stratégies de stockage et d'invalidation spécifiques

```csharp
public interface IGridJsJsonCache
```

## Méthodes

| Nom | Description |
| --- | --- |
| [ClearAll](../../aspose.cells.gridjs/igridjsjsoncache/clearall/)() | Effacer tous les caches |
| [GetCacheKey](../../aspose.cells.gridjs/igridjsjsoncache/getcachekey/)(string, string) | Générer une clé de cache. Les clients peuvent décider d'inclure ou non l'uid en fonction des exigences métier. - Si seul le nom de fichier importe : ignorez l'uid et utilisez uniquement fileName (recommandé, permet de partager le cache entre le même fichier). - Si la distinction de fichiers portant le même nom est requise : utilisez l'uid (mode strict). |
| [Invalidate](../../aspose.cells.gridjs/igridjsjsoncache/invalidate/)(string) | Invalider l'entrée de cache spécifiée. |
| [InvalidateAllForUid](../../aspose.cells.gridjs/igridjsjsoncache/invalidateallforuid/)(string) | Invalider toutes les entrées de cache contenant l'uid spécifié. Ceci est utile lorsque vous ne connaissez pas le fileName exact utilisé pour le cache. |
| [SetJson](../../aspose.cells.gridjs/igridjsjsoncache/setjson/)(string, string) | Écrire le JSON dans le cache. |
| [TryGetJson](../../aspose.cells.gridjs/igridjsjsoncache/trygetjson/)(string) | Essayer de récupérer le JSON depuis le cache. |

### Voir aussi

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


