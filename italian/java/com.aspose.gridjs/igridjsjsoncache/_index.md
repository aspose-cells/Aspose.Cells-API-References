---
title: "IGridJsJsonCache"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Interfaccia di cache JSON - i clienti implementano strategie di archiviazione e invalidazione specifiche"
type: docs
url: /it/java/com.aspose.gridjs/igridjsjsoncache/
---
```
public interface IGridJsJsonCache
```

Interfaccia di cache JSON - i clienti implementano strategie di archiviazione e invalidazione specifiche
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [clearAll()](#clearAll--) | Cancella tutte le cache |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) | Genera una chiave di cache. |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) | Invalidare la voce di cache specificata. |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) | Invalidare tutte le voci di cache contenenti l'uid specificato. |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) | Scrivi JSON nella cache. |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) | Tentare di recuperare JSON dalla cache. |
### clearAll() {#clearAll--}
```
public abstract void clearAll()
```


Cancella tutte le cache

### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public abstract String getCacheKey(String uid, String fileName)
```


Genera una chiave di cache. I clienti possono decidere se includere l'uid in base ai requisiti aziendali. - Se conta solo il nome del file: ignora l'uid e utilizza solo fileName (consigliato, consente la condivisione della cache tra file identici). - Se è necessario distinguere file con lo stesso nome: utilizza l'uid (modalità rigorosa).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | Identificatore univoco del file (può variare per caricamento). |
| fileName | java.lang.String | Nome file originale |

**Returns:**
java.lang.String - Chiave di cache
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public abstract void invalidate(String cacheKey)
```


Invalidare la voce di cache specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cacheKey | java.lang.String | Chiave di cache |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public abstract void invalidateAllForUid(String uid)
```


Invalidare tutte le voci della cache contenenti l'uid specificato. Questo è utile quando non si conosce il fileName esatto utilizzato per la cache.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | Identificatore univoco da corrispondere nelle chiavi di cache |

### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public abstract void setJson(String cacheKey, String json)
```


Scrivi JSON nella cache.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cacheKey | java.lang.String | Chiave di cache |
| json | java.lang.String | Stringa JSON |

### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public abstract String tryGetJson(String cacheKey)
```


Tentare di recuperare JSON dalla cache.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cacheKey | java.lang.String | Chiave di cache |

**Returns:**
java.lang.String - Stringa JSON se la cache è colpita, altrimenti null
