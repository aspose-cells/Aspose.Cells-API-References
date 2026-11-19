---
title: "IGridJsJsonCache"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Interface de cache JSON - les clients implémentent des stratégies de stockage et d'invalidation spécifiques"
type: docs
url: /fr/java/com.aspose.gridjs/igridjsjsoncache/
---
```
public interface IGridJsJsonCache
```

Interface de cache JSON - les clients implémentent des stratégies de stockage et d'invalidation spécifiques
## Méthodes

| Méthode | Description |
| --- | --- |
| [clearAll()](#clearAll--) | Effacer tous les caches |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) | Générer une clé de cache. |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) | Invalider l'entrée de cache spécifiée. |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) | Invalider toutes les entrées de cache contenant l'uid spécifié. |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) | Écrire le JSON dans le cache. |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) | Essayer de récupérer le JSON du cache. |
### clearAll() {#clearAll--}
```
public abstract void clearAll()
```


Effacer tous les caches

### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public abstract String getCacheKey(String uid, String fileName)
```


Générez une clé de cache. Les clients peuvent décider d'inclure le uid en fonction des exigences métier. - Si seul le nom du fichier importe : ignorez le uid et utilisez uniquement fileName (recommandé, permet de partager le cache entre les mêmes fichiers). - Si la distinction des fichiers portant le même nom est requise : utilisez le uid (mode strict).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | Identifiant unique du fichier (peut différer selon le chargement). |
| fileName | java.lang.String | Nom de fichier original |

**Returns:**
java.lang.String - clé de cache
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public abstract void invalidate(String cacheKey)
```


Invalider l'entrée de cache spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cacheKey | java.lang.String | Clé de cache |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public abstract void invalidateAllForUid(String uid)
```


Invalider toutes les entrées du cache contenant l'uid spécifié. Ceci est utile lorsque vous ne connaissez pas le fileName exact utilisé pour le cache.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | Identifiant unique à faire correspondre dans les clés de cache |

### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public abstract void setJson(String cacheKey, String json)
```


Écrire le JSON dans le cache.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cacheKey | java.lang.String | Clé de cache |
| json | java.lang.String | Chaîne JSON |

### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public abstract String tryGetJson(String cacheKey)
```


Essayer de récupérer le JSON du cache.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cacheKey | java.lang.String | Clé de cache |

**Returns:**
java.lang.String - Chaîne JSON si le cache est trouvé, null sinon
