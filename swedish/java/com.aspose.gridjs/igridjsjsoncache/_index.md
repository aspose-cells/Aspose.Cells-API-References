---
title: "IGridJsJsonCache"
second_title: "Aspose.Cells för Java API-referens"
description: "JSON‑cache‑gränssnitt – kunder implementerar specifika lagrings- och ogiltigförklaringsstrategier."
type: docs
url: /sv/java/com.aspose.gridjs/igridjsjsoncache/
---
```
public interface IGridJsJsonCache
```

JSON‑cache‑gränssnitt – kunder implementerar specifika lagrings- och ogiltigförklaringsstrategier.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [clearAll()](#clearAll--) | Rensa alla cachar |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) | Generera en cache-nyckel. |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) | Ogiltigförklara den angivna cacheposten. |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) | Ogiltigförklara alla cacheposter som innehåller den angivna uid:n. |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) | Skriv JSON till cache. |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) | Försök att hämta JSON från cache. |
### clearAll() {#clearAll--}
```
public abstract void clearAll()
```


Rensa alla cachar

### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public abstract String getCacheKey(String uid, String fileName)
```


Generera en cache-nyckel. Kunder kan besluta om de ska inkludera uid baserat på affärskrav. - Om endast filnamnet är viktigt: ignorera uid och använd endast fileName (rekommenderas, möjliggör delning av cache för samma fil). - Om det krävs att särskilja filer med samma namn: använd uid (strikt läge).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Unik identifierare för filen (kan skilja sig per laddning). |
| fileName | java.lang.String | Ursprungligt filnamn |

**Returns:**
java.lang.String - Cache-nyckel
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public abstract void invalidate(String cacheKey)
```


Ogiltigförklara den angivna cacheposten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cacheKey | java.lang.String | Cache-nyckel |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public abstract void invalidateAllForUid(String uid)
```


Ogiltigförklara alla cacheposter som innehåller den angivna uid. Detta är användbart när du inte vet det exakta fileName som används för cachning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Unik identifierare att matcha i cache-nycklar |

### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public abstract void setJson(String cacheKey, String json)
```


Skriv JSON till cache.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cacheKey | java.lang.String | Cache-nyckel |
| json | java.lang.String | JSON-sträng |

### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public abstract String tryGetJson(String cacheKey)
```


Försök att hämta JSON från cache.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cacheKey | java.lang.String | Cache-nyckel |

**Returns:**
java.lang.String - JSON-sträng om cacheträff, annars null
