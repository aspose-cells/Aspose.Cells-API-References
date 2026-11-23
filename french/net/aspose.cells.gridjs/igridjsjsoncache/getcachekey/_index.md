---
title: "IGridJsJsonCache.GetCacheKey"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IGridJsJsonCache. Générer une clé de cache. Les clients peuvent décider d'inclure ou non l'uid en fonction des exigences métier. Si seul le nom de fichier importe, ignorez l'uid et utilisez uniquement le nom de fichier, ce qui permet de partager le cache entre les mêmes fichiers. Si la distinction entre des fichiers portant le même nom est requise, utilisez l'uid en mode strict."
type: docs
url: /fr/net/aspose.cells.gridjs/igridjsjsoncache/getcachekey/
---
## IGridJsJsonCache.GetCacheKey method

Générer une clé de cache. Les clients peuvent décider d'inclure ou non l'uid en fonction des exigences métier. - Si seul le nom de fichier importe : ignorez l'uid et utilisez uniquement fileName (recommandé, permet de partager le cache entre le même fichier). - Si la distinction de fichiers portant le même nom est requise : utilisez l'uid (mode strict).

```csharp
public string GetCacheKey(string uid, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uid | String | Identifiant unique du fichier (peut différer à chaque chargement) |
| fileName | String | Nom de fichier original |

### Valeur de retour

Clé du cache

### Voir aussi

* interface [IGridJsJsonCache](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


